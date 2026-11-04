# SOOUA SEARCH 编译包

SOOUA Search 聚合搜索引擎的**站点编译包**（纯静态 H5）。下载部署到你自己的服务器并绑定域名，即可拥有与 [SOOUA 主站](https://www.sooua.cn) 同款的聚合搜索站点：AI / 网页 / 视频 / 小说 / 新闻 / 购物 / 图片 / 音乐等多源聚合搜索，外加直达、密令、热搜导航等能力。

## 下载

| 版本 | 编译包 | 说明 |
| --- | --- | --- |
| v110301 | [dist/sooua_search_110301.zip](dist/sooua_search_110301.zip) | 当前最新编译包 |

- 历史版本统一放在 [`dist/`](dist/) 目录
- 包内已内置站点验证标签，**无需修改任何代码**

## 相关链接

- 官方主站：https://www.sooua.cn
- 使用文档：https://doc.sooua.cn/index.php/article/5/936421724042297344.html
- 开放平台 · 免费部署教程：https://www.sooua.cn/index/open.html

## 截图

![首页](screenshots/wechat_longscreenshot_2026-11-02_230657_768.png)
![搜索结果](screenshots/wechat_longscreenshot_2026-11-02_230540_028.png)
![移动端](screenshots/wechat_longscreenshot_2026-11-02_230518_733.png)
![功能页一](screenshots/ScreenShot_2026-11-02_230636_415.png)
![功能页二](screenshots/ScreenShot_2026-11-02_230619_598.png)
![功能页三](screenshots/ScreenShot_2026-11-02_230608_058.png)

## 软件架构

- 前端为 Vue3 编译包，**纯静态文件，无后端依赖**，可部署在任意静态空间 / 虚拟主机（Nginx、Apache、PHP 空间、对象存储均可）
- 搜索、直达、密令等数据统一由 SOOUA 开放 API 提供，本地不存储任何业务数据
- 站点配置（标题、关键词、描述、LOGO、首页标语、备案号、统计代码、广告位、功能开关）全部在 SOOUA 个人中心云端管理，接口按域名自动下发，改完即时生效，无需重新部署

## 安装教程

1. 下载本仓库 [`dist/`](dist/) 目录下的最新编译包 `sooua_search_<版本号>.zip`
2. 解压后上传到你的网站根目录，绑定域名（建议配置 HTTPS）
3. 确认 `https://你的域名/` 能正常打开
4. 到 [SOOUA 个人中心](https://www.sooua.cn) 注册 / 登录 → 网站应用 → 新增应用，填写你的域名，点击「验证网站」（验证标签已内置在编译包中，无需修改任何代码）
5. 验证通过即完成接入，可正常使用全部免费功能

## 使用说明

1. 部署即可使用、无需维护、统一由官方维护，主要用于闲置域名、未备案域名、可挂广告
2. **自定义站点**：验证通过后即可在个人中心修改网站标题、关键词、描述、LOGO、首页标语（含链接）、ICP / 公安备案号、统计代码、广告位（推荐接入 [SOOUA 联盟](https://union.sooua.cn) 获取广告代码）
3. **版本更新**：个人中心网站应用列表常显「部署版本 / 最新版本」，版本过旧时会黄色提醒，点「下载最新版」获取新包重新上传覆盖即可

## 参与贡献

1. Fork 本仓库
2. 新建 Feat_xxx 分支
3. 提交代码
4. 新建 Pull Request

问题反馈与商务合作：微信 qq697553
