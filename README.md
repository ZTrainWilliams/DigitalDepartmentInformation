# digital-department-information

利用 Action 获取相关资讯文章（产品、运营、后端、前端、测试），每日定时推送到企微

## 方式
    利用[schedule](https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows#schedule)设置时间段定时，
    当前设置- cron: "29 23 * * *"，意思是UTC时间的第23个小时的第29分钟调用，大致北京时间8:30，实质上定时任务是会存在延迟的，可能服务器位置原因，毕竟免费资源
    当前项目如两个月无提交，schedule会自动关闭
    
## 咨询地址
``` javascript
const productNewsUrl = "https://www.woshipm.com/api2/app/article/popular/daily";
const csdnBlogUrl = 'https://blog.csdn.net/phoenix/web/blog/hot-rank?page=0&pageSize=25&type='
const frontNewsUrl = 'https://front-end-rss.vercel.app'
const testUtl = 'https://blog.csdn.net/nav/test'
```


## 其他

实现总结文章：
[Send-Font-News-Bot](https://github.com/ZTrainWilliams/Send-Font-News-Bot)
[基于GITHUB ACTION的定时任务，真香！](https://blog.csdn.net/qq_40748336/article/details/110749375)

[GitHub Actions 实现 RN App 自动化构建并推送到蒲公英](https://github.com/giscafer/blog/issues/53)
