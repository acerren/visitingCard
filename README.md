# AI名片小程序

## 版本说明

- mpvue 文件夹内的为 mpvue 版本的小程序
- native 文件夹内的为原生版本的小程序

请根据你自己的需要选择合适的版本，mpvue 版本将不再跟进维护，后续维护都将在原生版本上进行

## 介绍

本项目的 api接口及后台管理直接嫁接使用的 [api工厂](https://www.it120.cc/) 的免费云接口和云后台，在此先表示感谢！

本项目我们将会持续的维护下去，同时欢迎大家踊跃提交 ISSUE 或者加入进来一起开发和维护本项目！

## 接口 & 后台声明

本项目为纯前端项目，由于人力和精力所限，本项目并未有开发配套的后台系统，而是直接使用了 [api 工厂](https://www.it120.cc/) 提供的免费接口和后台，可以完全满足本项目的所有功能需求。

- [接口 SDK](https://github.com/gooking/apifm-wxapi)

- [免费后台](https://admin.it120.cc)

- [WeUI](https://github.com/Tencent/weui-wxss/)

## 扫码体验
<img src="https://cdn.it120.cc/apifactory/2018/12/18/c2324da4eea91602f385db5b523b13ca.jpg" width="200px">

## 其他开源模板

| 舔果果小铺 | 天使童装 | 面馆风格小程序 |
| :------: | :------: | :------: |
| <img src="https://cdn.it120.cc/apifactory/2018/04/01/b7b8f5a0fcfc72454ade8510ab929717.jpg" width="200px"> | <img src="https://cdn.it120.cc/apifactory/2019/06/28/a8304003-3218-4a47-95cf-84d82ebdc07b.jpg" width="200px"> | <img src="https://cdn.it120.cc/apifactory/2019/03/29/9e30cfe31eabcd218eb9c434f17e9295.jpg" width="200px"> | 
| [开源地址](https://github.com/walcer/TianguoguoXiaopu) | [开源地址](https://github.com/EastWorld/wechat-app-mall) | [开源地址](https://gitee.com/javazj/noodle_shop_procedures) |

## 联系作者

| 微信好友 | 支付宝好友 |
| :------: | :------: |
| <img src="https://cdn.it120.cc/apifactory/2019/07/03/a86f7e46-1dbc-42fe-9495-65403659671e.jpeg" width="200px"> | <img src="https://cdn.it120.cc/apifactory/2019/07/03/fda59aeb-4943-4379-93bb-92856740bd6a.jpeg" width="200px"> |

## QQ交流群

534721253 （可用手机QQ扫下面的二维码加群）

<img src="https://cdn.it120.cc/apifactory/2019/06/28/4f802bd3-6649-442a-a7a7-cc1a1196b5c7.png" width="200px">

## Mpvue版本使用说明

1、 [api工厂](https://www.it120.cc/) 右上角注册免费开通您的专属后台
> 
2、project.config.json  和 package.swan.json 文件中的 appid 改为你自己小程序的 appid；
> 
3、app.json 中的小程序名称和底部菜单名称改为你自己的；
> 
4、prod.env.js 文件中的小程序名称和专属域名换成你自己的；
> 
5、工厂后台，微信设置中，配置 appid 和 secret
> 
6、 [设置小程序合法服务器域名](https://www.yuque.com/apifm/doc/tvpou9)
> 
7、[系统参数设置](https://www.yuque.com/apifm/doc/kcncad)


## Mpvue版本编译并运行小程序

```bash
# 安装依赖
npm install
# 编译小程序
npm run dev
```
然后打开小程序的开发工具，导入本项目（当前项目下的  dist 文件夹下的wx文件夹）


## Native版本使用说明

1、 [api工厂](https://www.it120.cc/) 右上角注册免费开通您的专属后台
> 
3、config.js 中的subDomain 改成你自己专属域名即可；
> 
5、工厂后台，微信设置中，配置 appid 和 secret
> 
6、 [设置小程序合法服务器域名](https://www.yuque.com/apifm/doc/tvpou9)
> 
7、[系统参数设置](https://www.yuque.com/apifm/doc/kcncad)

## 初始化测试数据

登录后台，左侧菜单 “工厂设置” --> “数据克隆” --> “将别人的数据克隆给我”

对方商户ID填写  1708

点击 “立即克隆” ，然后退出后台重新登录

你将立即享有初始化测试数据，方便你进行测试

## 后台配置

1. 登录 [“api工厂”](https://www.it120.cc/) ，新注册一个用户；
2. 登录后，左侧菜单 “工厂设置” --> "模块管理",启用 "AI名片" 和 “系统参数” 模块,F5刷新后台；
3. 左侧菜单 “系统设置” --> “系统参数”，添加如下参数设置：
    - 开关类型参数: ALLOW_VIEW_FRIEND
      
      *设置为开启状态*
    - 文本类型参数: DEFAULT_FRIEND_UID

      *填写您希望的默认名片编号，填写后，以后用户打开你的小程序将默认展示该名片*
    - 文本类型参数: user.ext.fileds
  
      *填写默认的名片字段，多个字段用英文逗号分隔*

![如图所示](https://cdn.it120.cc/apifactory/2019/07/16/a0bd7ac8-5601-4bb7-b4ca-32d74e0ce273.png)

## 常见问题

### 如何添加名片 
- 登录后台，左侧菜单 “工厂设置” --> “模块管理” ，启用 “AI名片” 模块，然后退出重新登录后台你将可以看到名片的相关菜单
- 点击“访客管理”，选中某个用户给其分配名片
- 点击“名片管理”，你将能看到所有的名片信息
### 如何设置默认名片
- 设置默认名片后，任何用户进入小程序后，将会加载指定的某一张默认名片进行展示
- 首先你要启用“系统参数设置”模块，通过左侧菜单 “工厂设置” --> “模块管理”
- [系统参数设置](https://www.it120.cc/info/help/14152)
