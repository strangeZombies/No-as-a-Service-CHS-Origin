# ❌ 替你勇敢说不 No-as-a-Service-CHS-Origin

<p align="center">
  <img src="https://raw.githubusercontent.com/hotheadhacker/no-as-a-service/main/assets/imgs/naas-with-no-logo-bunny.png" width="800" alt="No-as-a-Service 横幅" width="70%"/>
</p>

有没有需要一种优雅的方式说“不”？  
这个小型 API 返回随机、通用、创意十足，有时还非常搞笑的拒绝理由——完美适用于任何场景：个人生活、职场、学生生活、开发者日常，或只是因为好玩。

为人类、借口和幽默而生。

---

## 🚀 API 使用

**基础 URL**  
```
https://naas.isalman.dev/no
```

**方法：** `GET`  
**速率限制：** `每 IP 每分钟 120 次请求`

### 🔄 示例请求
```http
GET /no
```

### ✅ 示例响应
```json
{
  "reason": "这感觉像是未来的我会因为现在的我同意而大喊大叫的事。"
}
```

可用于应用、机器人、登陆页面、Slack 集成、拒绝信，或任何需要礼貌（或机智）说“不”的地方。

---

## 🛠️ 自托管

想自己运行？它轻量且简单。

### 1. 克隆仓库
```bash
git clone https://github.com/hotheadhacker/no-as-a-service.git
cd no-as-a-service
```

### 2. 安装依赖
```bash
npm install
```

### 3. 启动服务器
```bash
npm start
```

API 将运行在：
```
http://localhost:3000/no
```

你也可以通过环境变量更改端口：
```bash
PORT=5000 npm start
```

---

## 📁 项目结构

```
no-as-service/
├── index.js            # Express API
├── reasons.json        # 1000+ 通用拒绝理由
├── package.json
├── .devcontainer.json  # VS Code / Github 开发容器设置
└── README.md
```

---

## 📦 package.json

供参考，以下是 package 配置：

```json
{
  "name": "no-as-service",
  "version": "1.0.0",
  "description": "一个返回随机拒绝或‘不’理由的轻量级 API。",
  "main": "index.js",
  "scripts": {
    "start": "node index.js"
  },
  "author": "hotheadhacker",
  "license": "MIT",
  "dependencies": {
    "express": "^4.18.2",
    "express-rate-limit": "^7.0.0"
  }
}
```

---

## ⚓ 开发容器

如果你在 Github Codespaces 中打开此仓库，`.devcontainer.json` 将自动设置你的环境。如果在 VSCode 中打开，它会询问是否在容器中重新打开。

---

## 使用 No-as-a-Service 的项目

以下是一些创意整合 [no-as-a-service](https://naas.isalman.dev/no) 以提供幽默或程序化“拒绝”响应的项目和网站：

1. **[no-as-a-service-rust](https://github.com/ZAZPRO/no-as-a-service-rust)**  
   本项目的 Rust 实现。

2. **[CSG Admins](https://csg-admins.de)**  
   一个系统管理和游戏服务中枢，使用 no-as-a-service 在某些管理面板和命令中提供幽默的否定响应。

3. **[FunnyAnswers - /no 端点](https://www.funnyanswers.lol/no)**  
   一个专注于幽默的 API 游乐场，包含 no-as-a-service 的镜像或包装器，非常适合探索有趣 HTTP 响应的开发者。

4. **[你的项目在此？](quare://github.com/YOUR_REPO)**  
   如果你在项目中使用 no-as-a-service，提交一个拉取请求以在此展示！

---

> 想在你的项目中使用 no-as-a-service？查看本 README 的使用部分，像专业人士一样返回“拒绝”。

---

## 👤 作者

由 [strangezombies](https://github.com/strangezombies) 使用ai二次翻译。

由 [hotheadhacker](https://github.com/hotheadhacker) 带着创意固执创建。

---

## 📄 许可证

MIT —— 随便做什么，就是别在该说“不”时说“是”。

---

**说明**：  
这是一个中文分支，翻译自英文 README，保留了原文的技术细节、结构和幽默语气，确保中文用户能够清晰理解 No-as-a-Service 的功能、使用方法和项目背景。所有链接和代码示例均保持原样，以便用户直接访问或使用。
