# 许美珍 · 乱世安_

**PHP + MySQL 后端 / Vue + TypeScript 前端** —— 专做中小型业务系统与管理后台。

晚上 18:30–23:30 接单，当晚响应，源码交付。

## 能接的活

| 方向 | 具体内容 |
| --- | --- |
| 企业管理后台 | 用户体系、角色权限（RBAC）、订单/库存/审批流、操作日志、数据字典、Excel/CSV 导入导出、报表与统计 |
| 第三方 API 对接 | 微信支付/支付宝、物流单号、短信、发票、企业微信/钉钉、ERP、快递鸟；签名加解密、幂等重试、失败告警 |
| 小程序 / App 后端 | 登录鉴权、下单支付、订单状态机，后台管理端，可配 Vue 前端一起交付 |
| 老系统接手改造 | ThinkPHP / Laravel / 原生 PHP 的历史代码接手，加功能、重构模块、清理临时方案 |
| MySQL 性能优化 | 索引设计、大表分表、统计查询卡顿、N+1 查询治理 |
| 数据处理脚本 | Excel/CSV 清洗合并、批量导入导出、对账脚本 |
| 大模型 API 接入 | 把现有系统接上 DeepSeek / 通义 / Kimi 等 OpenAI 兼容接口，智能客服、文本生成、报表解读，数据留在自己服务器 |
| 部署与运维 | 宝塔 / Nginx、Docker、CI/CD、备份定时任务、域名证书、迁移上线 |

## 项目

> 商业项目源码不便公开，这里放功能说明与技术要点。需要看细节可以单独约演示。

### 往事如书 · 面向老年人的 AI 回忆录 / 陪伴产品（全栈自研）

一套三端的完整产品：**PHP 后端 + Vue 用户端 + Vue 管理后台**。

- **后端 `memoir-run`**：PHP 8.2 + ThinkPHP 8 + MySQL。SSE 流式输出让 AI 回复逐字返回；接 OpenAI 兼容接口（DeepSeek）实现 AI 晚辈对话；百度 ASR 语音识别 + edge-tts 语音合成；回忆事件抽取；导出 Markdown / EPUB / PDF；家庭令牌鉴权与管理员鉴权中间件双轨隔离
- **用户端 `memoir-web-vue`**：Vue 3 + Vite + Vue Router，**不依赖 UI 框架**，自研设计令牌与轻量组件。AI 对话、跨会话/跨天的长期记忆、录音→识别→语音回复、回忆录时间轴与章节、大字号高对比的适老化无障碍设计
- **管理后台 `adminBook`**：Vue 3 + Vite 独立部署。家庭 / 成员 / 会话 / 回忆事件的数据管理与运营配置，`X-User-Token` 鉴权访问 `/api/v1/admin/*`

### 旭华小程序后台（PHP / ThinkPHP 6）

- **技术栈**：PHP 7.2+ / ThinkPHP 6 / ThinkORM 2 / MySQL
- **业务模块**：员工账号与令牌鉴权、订单管理、订单物流跟踪与轨迹详情、企业微信回调接入（WeWorkCallback）、订单备注
- **工程实践**：`.htaccess` 与 `nginx.htaccess` 双环境 URL 重写、`router.php` 兼容入口、`.example.env` 环境隔离、Travis CI、Composer 依赖锁定

### 生鲜水产小程序（微信小程序 / TypeScript）

- **技术栈**：微信小程序原生工程（TypeScript + SCSS）、`miniprogram-api-typings` 类型声明、ESLint + TypeScript 严格模式
- **业务模块**：登录、首页、商品下单、订单列表与全部订单、订单详情、订单备注、物流跟踪与轨迹详情、个人中心
- **工程实践**：微信开发者工具的工程配置与本地私有配置分离（`project.config.json` / `project.private.config.json`），独立的 `typings/` 类型目录

## 技术栈

```text
后端    PHP 7.2-8.2、ThinkPHP 6 / 8、ThinkORM、MySQL、Redis
前端    Vue 3 + Vite + Vue Router、JavaScript、TypeScript（自研设计令牌，不依赖 UI 框架）
小程序  微信小程序原生（TypeScript + SCSS）
工程    Nginx、Apache（.htaccess）、宝塔、Docker、Travis CI、Composer、Git
其他    大模型 API 接入（OpenAI 兼容）、SSE 流式、ASR 语音识别、TTS 语音合成
```

## 合作方式

- **远程优先**，晚上 18:30–23:30 固定在线，白天消息当天回
- **明码报价**，开工前先给工期与价格范围；不合适会直接说做不了，不硬接
- **交付含**：Git 私有仓库 → 分阶段验收 → 源码 + 数据库设计 + 部署文档 + 1 个月 bug 修复
- **第三方费用**（服务器、短信、地图 API 等）开工前说清谁承担，不事后追加

## 联系方式

- GitHub：https://github.com/xumeizhen001
- 微信 / 邮箱：见接单帖

