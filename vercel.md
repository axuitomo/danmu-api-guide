<div data-theme-toc="true"> </div>

>[!warning]
不要在国内媒体平台宣传danmu_api

>[!todo]
> 分解教程，多种搭建教程，细化教程

# 这是一份非官方的[danmu_api](https://github.com/huangxd-/danmu_api)搭建教程，

## 是否有必要搭建弹幕API

目前danmu_api支持 forward/senplayer/hills/小幻/yamby/eplayerx/afusekt/uz影视/dscloud/lenna/danmaku-anywhere/omnibox 等播放器。

搭配danmaku-anywhere可以实现为你的网页播放器提供好用的弹幕服务

> [danmaku-anywhere](https://github.com/Mr-Quin/danmaku-anywhere)旨在为你喜爱的几乎任何视频网站添加弹幕。通过添加自定义弹幕API例如danmu_api，可使用该插件为你的网页播放器提供弹幕。

## 最推荐的部署平台是Vercel和Netlify 【稳定，个人使用不会超额】
以下教程以Vercel为例

> ### [vercel部署及自动更新教程](https://github.com/xiaoyao20084321/log-var-danmu-deployment-guide)

> ### 优化点

* Settings > Functions > Advanced Setting > Function Region 切换为 新加坡/韩国/日本等，能提高访问速度，体验更优
  
  > hk 有可能访问不了 360 或其他源，可以尝试切其他 region
* vercel 在国内被墙，请配合代理或绑定自定义域名使用
  
  > 非必要教程-[使用 Vercel 搭建万能反向代理，部署后请绑定自定义域名使用](https://github.com/souying/vercel-api-proxy)

**推荐**：使用站内佬的edu.deal域名或者买一个xyz域名挂载到cloudflare，单域名SaaS优选再绑定

## 启用热更新

在Vercel中需设置变量：

**ADMIN\_TOKEN**    用于更改**系统变量**，消除日志等，自行设置
**DEPLOY\_PLATFROM\_PROJECT**
**DEPLOY\_PLATFROM\_TOKEN**

> **DEPLOY变量**可查看官方文档获取变量值——[各平台变量获取详细步骤](https://github.com/huangxd-/danmu_api/blob/main/danmu_api/ui/README.md#%E5%90%84%E5%B9%B3%E5%8F%B0%E5%8F%98%E9%87%8F%E8%8E%B7%E5%8F%96%E8%AF%A6%E7%BB%86%E6%AD%A5%E9%AA%A4)

访问域名/ADMIN\_TOKEN 进行下一步的变量设置 **例如**：https://danmu.8081666.xyz/ADMIN_TOKEN

## [UI界面变量设置](https://linux.do/t/topic/1461516#p-12586210-env-5)
