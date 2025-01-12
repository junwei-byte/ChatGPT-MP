## ChatGPT-MP(基于ChatGPT实现的微信小程序，适配H5和WEB端)

包含前后台，支持打字效果输出流式输出，支持AI聊天次数限制，支持分享增加次数等功能。**开源版禁止商用，仅供学习交流，禁止倒卖。** 感谢Star！

技术栈：JDK8 + SpringBoot + Vue2 + Uniapp + Mysql

Github地址：https://github.com/oldinaction/ChatGPT-MP

Gitee地址(国内访问更快)：https://gitee.com/smalle/ChatGPT-MP

小程序演示地址

![One能抽屉](https://cdn7.aezo.cn/common/qrcode/one_qrcode.jpg)


## 包含功能

- [x] ChatGPT聊天
- [x] 用户聊天次数限制
- [x] 分享得聊天次数
- [x] 每日领取免费次数
- [x] 查看聊天历史
- [x] 显示连接情况
- [x] 清除聊天历史
- [x] 开通会员
- [x] 购买次数包
- [x] 联系客服领取次数
- [x] 看广告得次数
- [x] 后台管理系统，暂时为升级版功能，之后会择机开源
- [x] 敏感词检测及设置
- [x] 适配H5和WEB端
- [x] 登录方式支持：小程序登录/微信公众号登录/手机号注册登录/邮箱注册登录
- [ ] AI生成图片、语音转换等功能开发中......

## 小程序/H5样式预览

小程序样式

<div align=left>
    <img src="images/MP-我的菜单.PNG" width="210" height="454"/>
    <img src="images/MP-聊天.PNG" width="210" height="454"/>
    <img src="images/MP-聊天历史.PNG" width="210" height="454"/>
</div>

H5登录注册界面，其他聊天界面类似小程序样式

<div align=left>
    <img src="images/H5-登录注册.PNG" width="210" height="454"/>
</div>

## 后端管理样式预览

<img src="images/用户管理.png"/>

<img src="images/用户次数管理.png"/>

<img src="images/敏感词管理.png"/>

<img src="images/数据统计.png"/>

## 开源版部署

### 后端

- 创建Mysql数据库aezo-chat-gpt, 执行脚本文件 aezo-chat-gpt-api/doc/aezo-chat-gpt.sql
- 使用IDEA打开aezo-chat-gpt-api项目
- 修改application.yml中的小程序id和秘钥、OpenAI地址和KEY
- 启动项目

**再加一点点说明：**

此项目开源后，收到了不少Star(感谢~)

其中不少同学非技术出身，很多都卡在后端项目启动这一步，我就将项目编译打包后的Jar一并上传了，之后只需安装好JDK并修改少许配置即可启动，省去了编译环节

Jar包启动方式如下：

1. 安装JDK(略)，网上教程较多
2. 下载dist.zip压缩包后进行解压
3. 修改此目录中的 application-dev.yml 文件(记事本文本编辑器即可打开，配置项已备注清楚)
4. 启动：Windows执行`start.bat`文件，Linux执行`start.sh`文件

### 前端小程序

- 使用HBuilder打开aezo-chat-gpt-m项目
- 修改common/config.js中的API地址
- 运行项目到微信小程序

## 版本功能比对

| 功能 | 开源版 | 升级版 |
|--|--|--|
| ChatGPT聊天 | ✅ | ✅ |
| 用户聊天次数限制 | ✅ | ✅ |
|  分享得聊天次数 | ✅ | ✅ |
| 每日领取免费次数 | ✅ | ✅ |
| 查看聊天历史 | ✅ | ✅ |
| 显示连接情况 | ✅ | ✅ |
| 清除聊天历史 | ✅ | ✅ |
| 开通会员 | ✅ | ✅ |
| 购买次数包 | ✅ | ✅ |
| 联系客服领取次数 | ✅ | ✅ |
| 看广告得次数 | ✅ | ✅ |
| H5/WEB端适配 | ❌ | ✅ |
| 敏感词过滤 | ❌ | ✅ |
| 后台管理-用户次数管理 | ❌ | ✅ |
| 后台管理-用户次数扣除历史 | ❌ | ✅ |
| 后台管理-敏感词管理 | ❌ | ✅ |
| 后台管理-发送消息统计 | ❌| ✅ |
| 后台管理-邀请人数统计 | ❌ | ✅ |
| 登录注册方式 | 小程序登录 | 小程序登录/微信公众号登录/手机号注册登录/邮箱注册登录 |
| 详细部署及使用文档 | ❌ | ✅ |
| 售后服务 | ❌ | 交流学习群 |

[升级版授权地址](https://ekey.aezo.cn/buy/1)

## 交流学习

有问题可进群交流，为了防止各种广告，需小额打赏1元以上~(你的心意就是我最大的动力)，添加请注明来意！

<details>
    <summary>点击查看联系方式（需小额打赏，添加注明OneChat）</summary>
    <img src="images/wechat-1.jpg" width="210" height="280" alt="微信：moonstarwall">
</details>

## 鸣谢

- 基于ChatGPT Java客户端[chatgpt-java](https://github.com/Grt1228/chatgpt-java)实现接口调用
