<p align="center"><img src="docs/images/readme-hero.svg?v=2" width="960" alt="让 ChatGPT 获得类似 Codex 的本地编程能力。Chat On Steroids：你的文件、终端和 ChatGPT 套餐。" /></p>

<p align="center">
  <a href="https://github.com/totec448-spec/chat-on-steroids/releases/latest/download/Chat-On-Steroids-Setup-x64.exe"><img src="docs/images/download-windows.svg" width="208" height="56" alt="下载 Windows x64 版本" /></a>&nbsp;
  <a href="https://github.com/totec448-spec/chat-on-steroids/releases/latest/download/Chat-On-Steroids-macOS-arm64.dmg"><img src="docs/images/download-macos.svg" width="208" height="56" alt="下载 macOS Apple 芯片版本" /></a>&nbsp;
  <a href="https://github.com/totec448-spec/chat-on-steroids/releases/latest/download/Chat-On-Steroids-Linux-x64.deb"><img src="docs/images/download-linux.svg" width="208" height="56" alt="下载 Linux x64 版本" /></a>
</p>

<p align="center"><a href="https://github.com/totec448-spec/chat-on-steroids/releases/latest">全部下载</a></p>

<p align="center"><sub>独立 Beta 测试版。使用风险由用户自行承担，并请遵守服务提供商的规则。连接前请阅读<a href="#负责任使用及服务提供商规则">使用说明</a>。</sub></p>

<br />

<p align="center"><a href="docs/images/demo.mp4"><img src="docs/images/demo.gif" width="960" alt="Chat On Steroids 演示：模型选择、任务计划、实时工具结果和可复用工作代理" /></a></p>

<p align="center"><a href="#开始使用">开始使用</a> &nbsp;·&nbsp; <a href="docs/images/demo.mp4">观看演示</a> &nbsp;·&nbsp; <a href="CHANGELOG.md">更新内容</a></p>

<br />

<h2 align="center">编程 · 分派任务 · 持续工作</h2>

**直接操作真实项目。** 让 ChatGPT 读取和编辑文件、运行测试、保持终端运行，并使用你的桌面。工具执行结果会实时显示。

**给它一个团队。** 可以把相互独立的工作分配给多个工作代理，再把结果汇总回来。每个代理都会保留自己的上下文，因此下一项任务可以从之前停止的位置继续。

**长任务也能保持控制。** 工作进行过程中仍可发送纠正指令。Goal 会继续处理尚未完成的工作；Loop 会在你的任务要求范围内持续工作；Compact & Resume 可以把当前会话及工作代理历史带入新的聊天。

<p align="center"><strong>本项目使用你的 ChatGPT 对话，而不是直接调用 Codex。</strong><br /><sub>ChatGPT Work 与 Codex 可能共享使用限制。你的账号可用模型、使用额度和上下文限制仍然适用。<a href="https://learn.chatgpt.com/docs/pricing">OpenAI 使用详情 →</a></sub></p>

## 负责任使用及服务提供商规则

Chat On Steroids 是一个独立的开源工作空间，用于在你自己的文件和工具上执行编程及其他经过授权的任务。它的设计目的，是帮助你在所使用服务的规则范围内提高工作效率。**它并不是用于绕过使用额度、账号限制或安全控制的工具。**

使用 CoS 时，请遵守 OpenAI 适用的[使用条款](https://openai.com/policies/terms-of-use/)（欧洲经济区、瑞士和英国请参阅[欧洲条款](https://openai.com/policies/eu-terms-of-use/)）、[使用政策](https://openai.com/policies/usage-policies/)和[服务条款](https://openai.com/policies/service-terms/)，同时遵守你的工作空间规则以及所有已连接服务的条款。

- **遵守额度与访问限制。** Workers、Goal/Loop、Compact & Resume 和完成检查点用于组织工作，并不会增加额度或模型访问权限，也不得用于规避速率限制、使用上限或账号限制。不要通过切换账号、聊天、连接器或隧道来规避限制。
- **遵守安全决定。** 如果服务提供商出于安全原因阻止某项操作，不要通过本地工具、浏览器控制、插件或其他工作代理绕过。获得本地权限或启用 MCP 连接器，并不代表可以覆盖服务提供商的拒绝。
- **了解集成方式。** CoS 通过 MCP 连接本地工具。配套组件还会观察并自动操作 ChatGPT 浏览器界面，并在本地记录对话内容。这种浏览器集成并不是公开的 ChatGPT 自动化 API。MCP 可用也不代表所有浏览器自动化或记录行为都获得许可；OpenAI 条款还会限制自动化或程序化提取数据或输出。
- **自行评估使用风险。** 连接前请查看账号规则和计划使用的工作流程；监督自动化过程，并检查工具执行动作和输出。CoS 无法保证政策合规、服务持续可用，也无法保证账号不会收到警告、限制或暂停。如果某个工作流程受到限制或收到政策警告，应停止该流程，并通过服务提供商的支持或申诉渠道寻求说明。

本说明仅描述项目的预期用途，并不构成合规认证，也不会改变任何服务提供商的规则。CoS 与 OpenAI 没有关联，也未获得 OpenAI 的认可或批准。软件按照 [MIT 许可证](LICENSE)以现状提供；适用的法定权利不受影响。本地权限及风险请参阅[安全说明](SECURITY.md)。

<br />

## 开始使用

1. **安装 CoS**，然后在 **Settings → Workspace（设置 → 工作空间）** 中批准你的项目文件夹。
2. 在 **Settings → Setup（设置 → 配置）** 中**连接 Core**，并在 ChatGPT 的开发者模式中添加它。[隧道配置 →](docs/setup.md#tunnel-setup)
3. **加载配套扩展。** 点击 **Open extension folder（打开扩展文件夹）**，然后在 Chrome 扩展程序设置中选择 **Load unpacked（加载已解压的扩展程序）**。配对会自动完成。
4. **选择模型，输入任务并发送。**

<details>
<summary>系统要求与安装说明</summary>

支持 Windows 10/11、**macOS 13 Ventura 或更新版本**，以及当前主流桌面 Linux。需要 Chrome 116+ 或当前版本 Edge，并需要一个支持开发者模式和自定义 MCP 应用的 ChatGPT 账号/工作空间。[检查账号是否支持](https://help.openai.com/en/articles/12584461-developer-mode-and-mcp-apps-in-chatgpt)。

- **未签名 Beta 版：** Windows 安装包没有发布者签名；macOS 版本也未签名、未公证。建议使用发布页面提供的校验值验证安装包。
- **Linux：** 需要 Secret Service 密钥环。优先使用 DEB；如果系统禁用了非特权用户命名空间，AppImage 启动器可以回退使用 <code>--no-sandbox</code>。
- **权限：** 连接之前请选择允许访问的文件夹并检查功能权限。全新安装默认启用 Core 功能和两个工作代理；Windows 还会启用 Desktop 桌面权限。Shell 命令以当前普通用户权限运行。
- **更新之后：** 根据提示重新加载配套扩展，并刷新 ChatGPT 中的 CoS 应用。

</details>

<details>
<summary>更多截图</summary>

![对话、工作代理和任务计划](docs/images/workspace.png)

![模型与推理强度选择](docs/images/model-picker.png)

![文件夹与功能权限设置](docs/images/settings.png)

</details>

<br />

---

<p align="center"><a href="docs/setup.md">安装与帮助</a> &nbsp;·&nbsp; <a href="docs/plugins.md">插件</a> &nbsp;·&nbsp; <a href="CONTRIBUTING.md">参与贡献</a> &nbsp;·&nbsp; <a href="SECURITY.md">安全说明</a> &nbsp;·&nbsp; <a href="LICENSE">MIT 许可证</a></p>

<p align="center">本项目由<a href="CONTRIBUTORS.md">社区贡献者</a>共同建设。感谢所有参与代码、设计、Bug 报告和测试的贡献者。</p>

<p align="center"><sub>本项目与 OpenAI 没有关联，也未获得 OpenAI 认可。ChatGPT 和 Codex 是 OpenAI 的商标。</sub></p>
