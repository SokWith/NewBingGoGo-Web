# NewBingGoGo-web

一个基于微软OpenAI ChatGPT GPT4的New Bing接口的Web服务。
提供了好看的对话页面。
实现了微软New Bing的大多数功能，还添加了一些自己的特色功能。
开源免费。

## 主要功能展示
### 聊天功能
聊天实现了NewBing的大多数功能，搜索，画图，天气，地图等等。
![1](https://github.com/jianjianai/NewBingGoGo-Web/assets/59829816/f951030f-7941-4ec7-887c-355d003a67be)

### 创作功能
创作实现了NewBing侧边栏的撰写的大多数功能，可更具需求生成文章。
![1 2](https://github.com/jianjianai/NewBingGoGo-Web/assets/59829816/c6469529-0571-4a5d-8161-1a9707f52592)

### 小窗功能 (插件专属)
小窗实现了NewBing侧边栏的根据当前页面信息问答的功能，可以在同一个页面中同时打开多个小窗同时问答，高效地查阅资料和完成文章编辑工作。
![1 1](https://github.com/jianjianai/NewBingGoGo-Web/assets/59829816/09d6cf75-f870-4c04-8809-70a3d7bc9817)


演示站点：
- repl java https://newbinggogo-web--jianjianai.repl.co (没配置账号)
- java https://chat.jja8.cn/ (加了一个我小号，轻掠)
- cloudflareWorker.js https://bingweb.jja8.cn/  (没配置账号)

## 功能介绍
此服务可直接通过网页访问也可以作为NewBingGoGo插件的魔法链接服务使用。

#### **直接访问** 
直接访问需要在配置文件中设置共享账号，可以设置多个共享账号随机访问。

#### **作为魔法链接**
作为魔法链接使用时，不会使用配置文件中的共享账号。用户需要登录自己的微软账号。


## 部署方法

[快速入门 wiki](https://github.com/jianjianai/NewBingGoGo-Web/wiki/%E5%BF%AB%E9%80%9F%E5%85%A5%E9%97%A8)

### 一键部署到免费的云服务器
|服务商 点击图标一键部署|简介|
|---|---|
|[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/GE_YVq?referralCode=s40fic)|Railway|
|[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/jianjianai/NewBingGoGo-Web)|Render|
|[![Deploy to Replit]()](https://replit.com/@jianjianai/NewBingGoGo-Web)|replit|


## 注意区分
### NewBingGoGo-web
NewBingGoGo-web是一个网页服务，用户可以直接打开网页，在网页上聊天。
但是由于网页的限制，用户是不能在网页上登录自己的微软账号的，必须使用服务端上配置的共享账号。

### NewBingGoGo
NewBingGoGo是一个浏览器插件，浏览器插件不同于网页，浏览器插件的权限更高。
所以在使用NewBingGoGo插件的时候，NewBingGoGo插件会从浏览器中自动获取当前登录的微软账号。

### NewBingGoGo-web 作为 NewBingGoGo 的魔法链接
NewBingGoGo-web既可以是一个网页服务，也可以是NewBingGoGo的魔法链接服务。当NewBingGoGo设置好魔法链接之后，就可以通过NewBingGoGo-web来代理聊天。
这个时候NewBingGoGo-web不会使用服务端上配置的共享账号，而是使用用户浏览器中当前登录的微软账号。

### 总结
搭建NewBingGoGo-web服务后，如果想直接打开网页使用则需要配置共享账号。如果仅仅作为NewBingGoGo的魔法链接使用则不需要配置共享账号。


## 关于
交流群：601156371


## 更加强大的NewBingGoGo插件
浏览器插件版的NewBingGoGo不受到网页的限制，更加强大。可以登录自己的微软账号，速度更快，更稳定。

[NewBingGoGo : 简单开始和NewBing聊天 gitee](https://gitee.com/jja8/NewBingGoGo)

| 功能     | 插件版 | web版 | 描述                                     |
|--------|-----|------|----------------------------------------|
| 聊天     | ✔   | ✔    | 和New Bing对话，提出问题。                      |
| 生成图片   | ✔   | ✔    | 在有更创造力选项中让New Bing生成图片                 |
| 提示词    | ✔   | ✔    | 使用提示词使AI更好地理解需求                        |
| 免登录    | ❌   | ✔    | 无需登录，直接使用。                             |
| 创作     | ✔   | ✔    | 使用New Bing生成文章，Edge浏览器New Bing侧边栏的撰写功能 |
| 小窗     | ✔   | ❌    | 在页面中打开小窗，可根据当前页面内容对话。Edge浏览器侧边栏的聊天功能   |
| 聊天记录   | ✔   | ✔    | 保存聊天记录，可查看或继续聊天                        |
| 登录微软账号 | ✔   | ❌    | 登录微软账号，使用自己的账号访问New Bing               |
| 内容卡片   | ✔   | ✔    | 显示天气，查找图片，地图等等。                        |
| 通过机器人验证| ✔ | ✔  | 当请求频繁时，微软要求通过机器人验证，就是输入验证码|


## 其他
暂时停更一段时间，6月10日之后继续更新。


{
    "conversationId": "51D|BingProdUnAuthenticatedUsers|07080C412AF5DF573614FD25E28C94C6A55D4A8F0E7D896C1EB7B2DCD62E5ADF",
    "clientId": "22E984E3F08C677022C095C4F15E668A",
    "conversationSignature": "3UFgrQhcY64Y9aaMKGEC0wt+At0GlGYal7bc/tZmdiE=",
    "result": {
        "value": "Success",
        "message": null
    }
}

cok5

MUID=22E984E3F08C677022C095C4F15E668A; SRCHD=AF=NOFORM; SRCHUID=V=2&GUID=3679F749CA9B423DB7967D76E4744CFE&dmnchg=1; _UR=QS=0&TQS=0; MMCASM=ID=D180BF6562CE4F29B75C853E4A54F339; MUIDB=22E984E3F08C677022C095C4F15E668A; _TTSS_IN=hist=WyJ6aC1IYW5zIiwiZW4iLCJhdXRvLWRldGVjdCJd; _tarLang=default=zh-Hans; _TTSS_OUT=hist=WyJwbCIsImVuIiwiemgtSGFucyJd; _EDGE_CD=m=en-us; GI_FRE_COOKIE=gi_sc=1; MicrosoftApplicationsTelemetryDeviceId=00174d61-21b0-4d0e-aee0-531a18222600; cct=UNd1piK6m1Z5e0ezaH_bc8i-zurdKUfLR8CkJBDnRbP8Ap9S4Z0BVKHth1PnK7LTRME3sGU63NpsC9OsOGLySw; _clck=1kfymad|2|fdy|0|1313; ABDEF=V=13&ABDV=13&MRNB=1691418357187&MRB=0; _HPVN=CS=eyJQbiI6eyJDbiI6MzcsIlN0IjoyLCJRcyI6MCwiUHJvZCI6IlAifSwiU2MiOnsiQ24iOjM3LCJTdCI6MCwiUXMiOjAsIlByb2QiOiJIIn0sIlF6Ijp7IkNuIjozNywiU3QiOjAsIlFzIjowLCJQcm9kIjoiVCJ9LCJBcCI6dHJ1ZSwiTXV0ZSI6dHJ1ZSwiTGFkIjoiMjAyMy0wOC0wN1QwMDowMDowMFoiLCJJb3RkIjowLCJHd2IiOjAsIkRmdCI6bnVsbCwiTXZzIjowLCJGbHQiOjAsIkltcCI6MTc0fQ==; ai_session=WYUDIwn2JMdKEaTeCp5wat|1691451481563|1691451481563; SRCHUSR=DOB=20200417&T=1691451473000; _EDGE_S=SID=0AF7D7C02EE566053401C4A62FCB67F6; SNRHOP=I=&TS=; NAP=V=1.9&E=1bc2&C=8EzIUD8iyDMU4KY_n2r9CtX0YKqpiZHX3sHbwzUV-_mJv_JO-LayNQ&W=1; SRCHS=PC=WSEDSE; USRLOC=HS=1&ELOC=LAT=34.04601287841797|LON=-118.24496459960938|N=%E6%B4%9B%E6%9D%89%E7%9F%B6%EF%BC%8C%E5%8A%A0%E5%88%A9%E7%A6%8F%E5%B0%BC%E4%BA%9A|ELT=1|&CLOC=LAT=38.4161|LON=112.7342|A=98021|TS=230807235100|SRC=I; _Rwho=u=d; ipv6=hit=1691455894181&t=4; WLS=C=&N=; SnrOvr=X=; GC=UNd1piK6m1Z5e0ezaH_bc8i-zurdKUfLR8CkJBDnRbOqclNLr60veAyEnSUnRNCq70QbfRlYBWV4n5TjHoAqwQ; _RwBf=W=0&ilt=2&ihpd=0&ispd=2&rc=10&rb=0&gb=0&rg=200&pc=5&mtu=0&rbb=0&g=0&cid=&clo=0&v=2&l=2023-08-07T07:00:00.0000000Z&lft=0001-01-01T00:00:00.0000000&aof=0&o=2&p=&c=&t=0&s=0001-01-01T00:00:00.0000000+00:00&ts=2023-08-07T23:52:25.9482579+00:00&rwred=0&wls=&wlb=&lka=0&lkt=0&TH=&dci=0; _SS=SID=0AF7D7C02EE566053401C4A62FCB67F6&PC=WSEDSE&R=10&RB=0&GB=0&RG=200&RP=5; SRCHHPGUSR=CW=927&CH=746&DPR=1.3&UTC=480&HV=1691452348&WTS=63815079910&DM=1&IPMH=3981989e&IPMID=1604652012338&SRCHLANG=zh-Hans&BRW=HTP&BRH=M&SW=1536&SH=864&PV=14.0.0&EXLTT=31&BZA=0&PRVCW=927&PRVCH=746&AV=14&ADV=14&RB=0&SCW=1164&SCH=3725&THEME=1&PR=1.25&IG=A915406808E84A93AEB8A09367852AA2&cdxtone=Creative&cdxtoneopts=h3imaginative,clgalileo,gencontentv3,fluxsrtrunc,fluxtrunc,fluxv1,rai278,replaceurl&CMUID=22E984E3F08C677022C095C4F15E668A



coksw02-30


MUID=22E984E3F08C677022C095C4F15E668A; SRCHD=AF=NOFORM; SRCHUID=V=2&GUID=3679F749CA9B423DB7967D76E4744CFE&dmnchg=1; _UR=QS=0&TQS=0; MMCASM=ID=D180BF6562CE4F29B75C853E4A54F339; MUIDB=22E984E3F08C677022C095C4F15E668A; _TTSS_IN=hist=WyJ6aC1IYW5zIiwiZW4iLCJhdXRvLWRldGVjdCJd; _tarLang=default=zh-Hans; _TTSS_OUT=hist=WyJwbCIsImVuIiwiemgtSGFucyJd; _EDGE_CD=m=en-us; GI_FRE_COOKIE=gi_sc=1; MicrosoftApplicationsTelemetryDeviceId=00174d61-21b0-4d0e-aee0-531a18222600; cct=UNd1piK6m1Z5e0ezaH_bc8i-zurdKUfLR8CkJBDnRbP8Ap9S4Z0BVKHth1PnK7LTRME3sGU63NpsC9OsOGLySw; _clck=1kfymad|2|fdy|0|1313; ABDEF=V=13&ABDV=13&MRNB=1691418357187&MRB=0; ai_session=WYUDIwn2JMdKEaTeCp5wat|1691451481563|1691451481563; SNRHOP=I=&TS=; SRCHS=PC=WSEDSE; USRLOC=HS=1&ELOC=LAT=34.04601287841797|LON=-118.24496459960938|N=%E6%B4%9B%E6%9D%89%E7%9F%B6%EF%BC%8C%E5%8A%A0%E5%88%A9%E7%A6%8F%E5%B0%BC%E4%BA%9A|ELT=1|&CLOC=LAT=38.4161|LON=112.7342|A=98021|TS=230807235100|SRC=I; _Rwho=u=d; ipv6=hit=1691455894181&t=4; GC=UNd1piK6m1Z5e0ezaH_bc8i-zurdKUfLR8CkJBDnRbOtwUW60Rx1Fm5z3C5yOndLl-PVOzvz0ZW6jHZ6iON-Ag; CSRFCookie=b45ad19a-343a-480b-8c54-77707ea0c26b; SRCHUSR=DOB=20200417&T=1691451473000&POEX=W; ANON=A=F20B8A374585DC1CDEFF5630FFFFFFFF&E=1caa&W=a; NAP=V=1.9&E=1c50&C=lY_12nDB0kIOyK0J1NF7Uynn4w3KH5BMH8ToHBSDm1Fz5EdFRBb0yw&W=6; PPLState=1; KievRPSSecAuth=FAByBBRaTOJILtFsMkpLVWSG6AN6C/svRwNmAAAEgAAACKK7iO7OzKB9MASFDuB+pvLnKZfvcDu2JZkmNlgXlepbYPYE7V0AU7NgdX354okiDQQj8bd5JAHxFOC6E6rYaxlF9RtScWmqWMcQj/E77Ykf7G/7iVzyAnDTVKKZNR45fHKSKgGHYSn3exlSoj2657FbzEFaQ0ocgBYLeaLXRP5oehv+jSoqYg0hRuK6u2qDXh9WvTJnxmSEXo3FvhRl9Nd1HgCc8R1WzkPWmbomDusaovv3NuXRQn18Jcepa83l+QvOnnnuGnYB/PlFhPwD/omtjWH/DTKqOpNc73ltWHnJPrSIKeaKMKwDOBa7TOB1HLQ6SiYOCyIYoUOH3F07lTUUYUuZJAPmCfGNxOl5EyyPo88LG8sU6aPZ1RT9I/RwHNsf3g+eGa3ju5spQPxZy6pDUwpjsruuMC6JWx2YFUbC3PsNRg+NQ3BNpFknrz8kun0T1jTM5FdfMOtlqZwjQssx4UAz2nCgYqnVi+s9qX0nvqoqd/7zaCGO2nUgnFCsmvqs2EJpNF17OP1XhbcfV+OhANZ7jvFx9iwhIgGnwQXB5o7PxCenSHbauBpFX5eQcHDmqZcrPsItBARuNQm4cDf5ggYoyJhfHP5oylmwzgHw/1WhV+ab4uCapA5Nj6TBncVEZyZhKgeV4wOm6f6CYTnOC6yUskUWwqQn0bBnWvFajA0RXE0SfPoD7a0PzYXYaU1ZmPCyjUreqU8aX1g0ca5yyobD4K+IylzRF1f9SlKg8EH+FFmrXJS9VWuCA8x+79SFq8ldljq+UiqYWvJqMB89772TCNhkBX2y83ydSr+IgJS3Kknhhy04t35NqwmDaKfKovymGEs4J6TYAQWIO567DzfdoYXsSnU5pkrJu//vw01UQvnNHiFoJ4xlNULXCd5N2VWWFCmjmHUQeikkweBMdiMo4igB3aHpDwEEnZyS2R1xApfJ0iqUnujyqXIxfNVI8Zzy50eRFkeREgJ76WtXZwGw22bTDyCYeqHk67fJxtFBZX6ahiftF1NkYNPCrk4Ehd/d4Fqaz1MTY2Tx1cftXWvTs8OySb00z6LxHeTnblXA6MsrAv/NZbdUChKp5JkZlVqBLE2DneZFPMmdoZxFX+5baaDLiG34oCP86v/j/yEzCNakAA3mM86OirTM4CCQL7/RQBhFosNhjv2zTqA3zcPsNHTCCkIMfdtPV3ERb5ZIvozlo9Pnkxt8NPYGrS7BE5rLmNEUdQDwtqZF4oq/3NH+pzgwJ6h66RKgHHtWqU3FyChwDmyURi/Q2xfLF/lK20850dGMrCegT8YkR2qdp2Ss82UYVp849lSqxZBBTn0iSPKd86uNYCcTOrxNGBjAXGNBag7Tpf/RhmBBKiYe6V4pojS+Fr/i1mDRaN+rK/JPU41Q4TdKUArBqG+hFxtVL3ublGAE36Wcl1juybpyldBJ81EYydTqFAApKKtA9UcYa/OobIx+cOeHKC0DgQ==; _U=10_7di1iHXuZxiJI1c_tEcsuoNj9UOJDEIx_N0VdC_7fTYY6ivk6KDk3XlIZEU9JYa7HFT7-oKNM557yVLpmgFpdhI07GiE0_osB7GX-yWkWFA2l8_RbwDNpbg0RWIG6Wj9_w4kIssHYvnUVidwEjPYRO2pEmMdlQ_CslKleTzVV1ywVxL-VVDPPMRkz9OAVC2b1LAhvHIUGdKemVsoKe-G9WZ4E-RsnV1R1SQrKhXjs; WLS=C=1c94711e1db4da5d&N=sokwith; WLID=abZLFPAGUD+oYOBjigmpe+0XHq6a1dLmQCJbztR1pvbTKEk3uwP+QgsNWSBp5LXq/GcwITJcHRt2qSwRxNx+Jcjdn1jUQLyfCGccblBMvGc=; SUID=A; _EDGE_S=SID=333A6D112BC865C00B7D7E772AA764AC&mkt=en-us; _SS=SID=0AF7D7C02EE566053401C4A62FCB67F6&PC=WSEDSE&R=19&RB=19&GB=0&RG=0&RP=10; SnrOvr=X=rebateson; _HPVN=CS=eyJQbiI6eyJDbiI6MzcsIlN0IjoyLCJRcyI6MCwiUHJvZCI6IlAifSwiU2MiOnsiQ24iOjM3LCJTdCI6MCwiUXMiOjAsIlByb2QiOiJIIn0sIlF6Ijp7IkNuIjozNywiU3QiOjAsIlFzIjowLCJQcm9kIjoiVCJ9LCJBcCI6dHJ1ZSwiTXV0ZSI6dHJ1ZSwiTGFkIjoiMjAyMy0wOC0wN1QwMDowMDowMFoiLCJJb3RkIjowLCJHd2IiOjAsIkRmdCI6bnVsbCwiTXZzIjowLCJGbHQiOjAsIkltcCI6MTc1fQ==; _RwBf=W=1&ilt=2&ihpd=0&ispd=2&rc=19&rb=19&gb=0&rg=0&pc=10&mtu=0&rbb=0.0&g=0&cid=&clo=0&v=3&l=2023-08-07T07:00:00.0000000Z&lft=0001-01-01T00:00:00.0000000&aof=0&o=0&p=BINGCOPILOTWAITLIST&c=MR000T&t=607&s=2023-07-23T08:43:32.8162788+00:00&ts=2023-08-07T23:55:33.2865551+00:00&rwred=0&wls=2&wlb=0&lka=0&lkt=0&TH=&dci=0&r=1&mta=0&e=1DID_69N_EojDsKdhJWE6ACexvDTECfYvwPBQtOJoSvU8c88u7By-Xiuno-54Yt9djib5x-qgn1Glr8JWqtv4wIvpXYN52XSGTO1hg9AsGo&A=F20B8A374585DC1CDEFF5630FFFFFFFF; SRCHHPGUSR=CW=494&CH=746&DPR=1.3&UTC=480&HV=1691452534&WTS=63815079910&DM=1&IPMH=3981989e&IPMID=1604652012338&SRCHLANG=zh-Hans&BRW=NOTP&BRH=M&SW=1536&SH=864&PV=14.0.0&EXLTT=31&BZA=0&PRVCW=1482&PRVCH=746&AV=14&ADV=14&RB=0&SCW=1164&SCH=3699&THEME=1&PR=1.25&IG=A915406808E84A93AEB8A09367852AA2&cdxtone=Creative&cdxtoneopts=h3imaginative,clgalileo,gencontentv3,fluxsrtrunc,fluxtrunc,fluxv1,rai278,replaceurl&CMUID=22E984E3F08C677022C095C4F15E668A

