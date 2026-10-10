# 财务人 SKILL 速查手册模板

这是一个可以直接修改的静态网页模板。解压后双击 `index.html` 即可本地预览，不需要安装 Node、数据库或服务器。

## 快速定制

1. 用 VS Code、记事本或其他编辑器打开 `index.html`。
2. 搜索并修改品牌名称、版本号、技能数量、抖音名称、抖音号和推广语。
3. 修改 `<section class="module">` 里的分类和卡片。每张卡片包含技能名称、`skill-id`、用法、场景和复制按钮。
4. 在 `samplePrompts` 中用相同的 `skill-id` 修改对应提问样例；否则卡片会使用通用样例。
5. 如需更换头像，将图片放入 `assets` 目录，并修改 `creator-profile` 中的图片路径和替代文本。
6. 如需删减或增加本地技能，编辑 `skills` 目录中的 `SKILL.md`，并同步卡片的 `skill-id` 和安装来源映射。
7. 用浏览器重新打开 `index.html` 检查搜索、提问样例、复制、置顶和安装指令。

## 重新打包

在模板根目录打开 PowerShell，执行：

```powershell
Compress-Archive -Path index.html,README.md,CUSTOMIZE.md,assets,skills -DestinationPath .\my-finance-skill-manual.zip -Force
```

不要把 `.git`、临时文件或包含密码/API Key 的文件放进压缩包。发布前请用脱敏内容测试，并自行核对技能来源、许可证、依赖和费用。

## 安装技能

网页中的安装指令只负责让 Agent 检查来源、依赖和兼容性。不要把未核验的技能直接安装到生产环境；需要 WorkBuddy 时，让 Agent 准备 ZIP 后在技能页面导入。
