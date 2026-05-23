# session-to-authjson

A static HTML converter for turning a ChatGPT session JSON export into an auth JSON shape.

Online page:

```text
https://fengfengzhidao.github.io/session-to-authjson/
```

You can also open [index.html](./index.html) directly in a browser. Paste the source JSON and convert it locally. The page does not send tokens anywhere and does not store them in local storage.

## 原理

Codex 本地读取的 `auth.json` 如果已经包含有效登录状态，启动时就可以直接使用这份状态，不会重新进入登录流程。

ChatGPT 网页端登录成功后，浏览器里会有一份可用的网页登录状态。这个工具做的事情就是把网页端已有的登录状态字段转换成 Codex 本地 `auth.json` 需要的格式。

这个工具不会破解、生成或刷新 token，也不会跳过账号本身要求的验证流程；它只适合转换你自己已经合法登录得到的会话信息。

## GitHub Pages

This repository publishes the static page from the `gh-pages` branch.

In repository **Settings -> Pages**, choose:

- Source: `Deploy from a branch`
- Branch: `gh-pages`
- Folder: `/ (root)`
