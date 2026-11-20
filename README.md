# Hide Office Upgrade Button

**隐藏 Microsoft Office「升级计划」按钮**

[简体中文](#简体中文) | [English](#english)

---

## 简体中文

### 项目简介

部分 Microsoft Office 用户会在 Word、Excel、PowerPoint 的右上角看到「升级计划」按钮，且无法通过常规设置隐藏。

本项目通过修改 Windows 注册表中的 Office 功能开关，尝试隐藏该按钮，并提供恢复脚本，方便用户撤销修改。

### 功能特点

- 隐藏 Office 右上角的「升级计划」按钮
- 支持 Word、Excel、PowerPoint
- 无需安装第三方软件
- 无需修改 Office 程序文件
- 不禁用 Office 自动更新
- 不修改 Office 激活或许可证信息
- 提供恢复默认配置的注册表文件

### 兼容性

| 项目 | 支持情况 |
|---|---|
| Windows 10 / 11 | 适用平台 |
| Office 2021 | 有社区成功反馈 |
| Office 2024 | 有社区成功反馈 |
| Microsoft 365 | 部分版本有成功反馈 |
| Word | 支持尝试 |
| Excel | 支持尝试 |
| PowerPoint | 支持尝试 |

**注意：** 不同 Office 版本及更新通道的实际效果可能不同，无法保证所有版本有效。

### 使用方法

**1. 关闭 Office**

完全退出所有 Word、Excel、PowerPoint 窗口。

**2. 备份注册表**

建议先使用注册表编辑器备份 Office 对应配置，或创建系统还原点。

**3. 隐藏升级按钮**

下载并双击：

`hide-upgrade-button.reg`

确认注册表导入操作。

**4. 重新启动 Office**

再次打开 Word、Excel 或 PowerPoint，检查右上角的按钮是否消失。

### 如何恢复默认设置

如果需要撤销修改：

1. 关闭所有 Office 应用程序。
2. 双击 `restore-default.reg`。
3. 确认导入注册表。
4. 重新启动 Office。

恢复脚本将删除本项目使用的功能覆盖值，使 Office 重新使用默认配置。

需要注意，如果修改前这些注册表值已经存在，恢复脚本无法重建原有的自定义值，应使用事先保存的注册表备份完成精确恢复。

### 注意事项

- 本项目仅修改当前 Windows 用户的注册表。
- 不涉及 Office 文件修改、破解或激活。
- Office 后续更新可能改变相关功能开关的行为。
- 修改注册表存在风险，请先备份重要配置。
- 本项目为非官方社区解决方案，不保证适用于所有 Office 版本。

---

## English

### Overview

Some Microsoft Office installations display a persistent **"Upgrade your plan"** button in the upper-right corner of Word, Excel, and PowerPoint.

This project provides a lightweight Windows Registry workaround that attempts to hide the button without modifying Office program files.

A restoration script is also included.

### Features

- Hide the "Upgrade your plan" button
- Support Word, Excel, and PowerPoint
- No third-party software required
- No Office executable modifications
- No need to disable Office automatic updates
- No changes to Office activation or licensing
- Includes a restoration script

### Compatibility

| Product | Compatibility |
|---|---|
| Windows 10 / 11 | Target platform |
| Office 2021 | Community-reported success |
| Office 2024 | Community-reported success |
| Microsoft 365 | Works on some reported versions |
| Word | Targeted |
| Excel | Targeted |
| PowerPoint | Targeted |

**Note:** Compatibility depends on the Office version, build, and update channel. Results are not guaranteed.

### Installation

**Step 1: Close Office applications**

Exit Word, Excel, and PowerPoint completely.

**Step 2: Back up your registry**

Create a registry backup or Windows restore point before applying any changes.

**Step 3: Apply the registry tweak**

Download and double-click:

`hide-upgrade-button.reg`

Confirm the Registry Editor prompt.

**Step 4: Restart Office**

Open Word, Excel, or PowerPoint and check whether the button has disappeared.

### Restore Default Settings

To revert the changes:

1. Close all Office applications.
2. Double-click `restore-default.reg`.
3. Confirm the registry import.
4. Restart Office.

This removes the feature overrides introduced by the project, allowing Office to use its default behavior again.

The restore script does not reconstruct custom registry values that may have existed before installation. Use your original registry backup if an exact rollback is required.

### Disclaimer

This project is an unofficial community workaround and is not affiliated with or endorsed by Microsoft.

Microsoft may change these internal settings in future Office updates.

Back up your registry before making modifications. Use this project at your own risk.

---

## References / 参考资料

- [Original community registry workaround](https://gist.github.com/cruithne3753/d7ebf2f11203635f5ba7478b4de3600c)
- [Microsoft Q&A discussion](https://learn.microsoft.com/en-us/answers/questions/5976610/how-can-i-permanently-remove-the-upgrade-your-plan)
