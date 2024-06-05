# Git Graph 扩展 for Visual Studio Code

You can also read this README in [简体中文](https://github.com/TiAmo-chen/vscode-git-graph_zh-cn/blob/develop/README_ch-cn.md)

在 Visual Studio Code 中查看你的仓库的 Git 图，并能直接从图表上轻松执行 Git 操作。可配置以满足你的显示需求！

![Git Graph 录制演示](https://github.com/mhutchie/vscode-git-graph/raw/master/resources/demo.gif)

## 功能

### Git Graph 视图
- **显示**：
  - 本地与远程分支
  - 本地引用：头、标签和远程
  - 未提交的更改
- **执行 Git 操作**（通过右击提交/分支/标签）：
  - 创建、检出、删除、拉取、合并、推送、变基、重命名和重置分支
  - 添加、删除和推送标签
  - 检出、挑选、丢弃、合并和还原提交
  - 清理、重置和暂存未提交更改
  - 应用、从暂存创建分支、丢弃和弹出暂存
  - 查看注解标签详情（名称、邮箱、日期和消息）
  - 复制提交哈希、分支、暂存和标签名称到剪贴板
- **点击提交查看详细信息和文件更改**：
  - 点击任意文件更改查看 VS Code 差异
  - 打开提交中受影响文件的当前版本
  - 复制受影响文件路径到剪贴板
  - 点击提交正文中的 HTTP/HTTPS 链接，在默认浏览器中打开
- **比较任意两提交**：通过点击一个提交，然后使用 CTRL/CMD 加点击另一个提交进行比较
- **代码审查**：跟踪在提交详情和比较视图中已审查的文件
- **查看未提交更改，并与任何提交比较**
- **悬停提示**：鼠标悬停在图表上的任何提交顶点上，查看包含以下信息的工具提示：
  - 提交是否包含在 HEAD 中
  - 哪些分支、标签和暂存包含该提交
- **过滤显示的分支**：使用“分支”下拉菜单。选项包括：
  - 显示所有分支
  - 选择一个或多个分支查看
  - 选择用户预定义的自定义 glob 模式数组（通过设置 `git-graph.customBranchGlobPatterns`）
- **从远程拉取**：（在顶部控制栏可用）
- **查找工具**：快速查找包含特定短语的一个或多个提交
- **仓库设置工具**：
  - 查看、添加、编辑、删除、拉取和清理远程仓库
  - 配置“问题链接”——将提交消息中的问题编号转换为超链接，直接在问题追踪系统中打开问题
  - 配置“拉取请求创建”——直接从分支上下文菜单自动打开并预填充拉取请求表单
  - 内置对公有 Bitbucket、GitHub 和 GitLab 拉取请求提供商的支持
  - 可配置自定义拉取请求提供商（例如，私有拉取请求提供商）。配置自定义提供商的信息可在此处找到：[链接](https://github.com/mhutchie/vscode-git-graph/wiki/Configuring-a-custom-Pull-Request-Provider)
  - 导出 Git Graph 仓库配置到文件，可在仓库中提交，使同一仓库的其他协作者自动使用相同的 Git Graph 配置
- **键盘快捷键**：
  - `CTRL/CMD + F`：打开查找工具
  - `CTRL/CMD + H`：滚动到 HEAD 引用的提交
  - `CTRL/CMD + R`：刷新 Git Graph 视图
  - `CTRL/CMD + S`：滚动到第一个暂存
  - `CTRL/CMD + SHIFT + S`：滚动到最后一个暂存
  - 在提交详情视图中：
    - 上/下箭头：在 Git Graph 视图上打开相邻的提交详情
    - `CTRL/CMD + 上/下箭头`：在同一条分支上打开子或父提交
    - 按住 Shift 键（即 `CTRL/CMD + SHIFT + 上/下箭头`）时，遇到分支或合并会跟随另一条分支
- **Enter**：提交对话框，按下 Enter 提交主要操作
- **Escape**：关闭活动对话框、上下文菜单或提交详情视图
- 列宽调整，显示/隐藏日期、作者和提交列
- 自动替换提交消息中的常见 Emoji 简码为对应表情（包括所有 [gitmoji](https://gitmoji.carloscuesta.me/)）。自定义 Emoji 简码映射可在 `git-graph.customEmojiShortcodeMappings` 中定义。

### 配置设置
- 包括图形样式、分支颜色等广泛配置。详细信息见“扩展设置”部分。

### 启动方式
- 状态栏上的“Git Graph”启动按钮
- 命令面板中的“Git Graph: View Git Graph”命令

## 扩展设置
- 详细设置说明、截图、默认值和类型，请参阅[这里](https://github.com/mhutchie/vscode-git-graph/wiki/Extension-Settings)。

## 扩展命令
- 提供了多个命令，如查看 Git Graph、添加/移除 Git 仓库、清除头像缓存、处理代码审查等。

## 发布说明
- 详细发布说明请见[CHANGELOG.md](CHANGELOG.md)。

## Visual Studio Marketplace
- 该扩展在[Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph)上提供。

## 致谢
- 感谢所有帮助开发 Git Graph 的贡献者！
- 使用的部分图标来自以下来源，请支持他们的优秀工作：
  - [GitHub Octicons](https://octicons.github.com/)（[许可](https://github.com/primer/octicons/blob/master/LICENSE)）
  - [Icons8](https://icons8.com/icon/pack/free-icons/ios11)（[许可](https://icons8.com/license)）