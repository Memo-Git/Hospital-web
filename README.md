# SparkCareNexus 医院端静态预览

本仓库只存放 **SparkCareNexus 医院端** 的前端静态预览产物，用于 GitHub Pages 打开。它是纯前端 Mock 原型，**不是生产系统**，没有真实后端、鉴权或医院数据。

源码不在本仓库。请勿把 `node_modules`、源码或本地日志提交进来。

## 如何开启 GitHub Pages

1. 打开本仓库的 GitHub 页面。
2. 进入 **Settings → Pages**。
3. **Build and deployment → Source** 选择 **Deploy from a branch**。
4. **Branch** 选择默认分支（当前为 `main`）。
5. **Folder** 选择 **`/ (root)`**（不要选 `/docs`）。
6. 保存后等待一两分钟，直到 Pages 状态变为已发布。

访问地址（Hash 路由）：

- 站点：https://memo-git.github.io/Hospital-web/
- 登录页：https://memo-git.github.io/Hospital-web/#/login

首次打开若仍是空白页，请确认 Folder 选的是 `/ (root)`，并且仓库根目录有 `index.html` 和 `.nojekyll`。

## 演示登录

1. 打开 `#/login`。
2. 输入账号后，先点击 **获取验证码**（Mock 会自动填入验证码）。
3. 输入密码，再点击登录。

| 账号 | 密码 | 说明 |
| --- | --- | --- |
| `admin` | `admin` | 医院主账号 |
| 分账号（如 `appointment.staff`） | `123456` | 默认分账号密码 |

未先获取验证码会提示验证码失效。

## 说明

- 本预览使用 Hash 路由（地址形如 `/Hospital-web/#/dashboard`），刷新子路径不会 404。
- 页面数据均为前端 Mock，仅供界面与流程演示。
