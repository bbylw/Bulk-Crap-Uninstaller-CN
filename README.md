[![捐赠](https://img.shields.io/badge/donate-paypal-brightgreen.svg)](http://klocmansoftware.weebly.com/donate.html)
[![GitHub 版本](https://img.shields.io/github/release/klocman/Bulk-Crap-Uninstaller.svg)](https://github.com/Klocman/Bulk-Crap-Uninstaller/releases)
[![许可证](https://img.shields.io/github/license/klocman/Bulk-Crap-Uninstaller.svg)](https://github.com/Klocman/Bulk-Crap-Uninstaller/blob/master/Licence.txt)

### [:warning: 正在寻找维护者 :warning:](https://github.com/Klocman/Bulk-Crap-Uninstaller/discussions/289)

# Bulk Crap Uninstaller
Bulk Crap Uninstaller（简称 BCUninstaller）是一款自由（言论自由意义上的）程序卸载工具。它擅长以最少的用户操作批量卸载大量应用程序。它可以清理残留文件、检测孤立应用、根据预设列表运行卸载程序，还有更多功能！尽管 BCU 是为 IT 专业人员设计的，但任何对 Windows 中应用程序安装/卸载有基本了解的人都可以使用。

BCU 完全兼容 Windows 应用商店应用、Steam、Windows 功能，并对多种卸载系统（NSIS、InnoSetup、Msiexec 等）提供特殊支持。请查看下方的完整功能列表。

Bulk Crap Uninstaller 采用 Apache 2.0 开源许可证，只要遵守许可证条款，即可免费用于私人和商业用途，没有任何义务。

[访问官方主页](https://www.bcuninstaller.com/) 查看完整的特性和功能列表！

如果您有任何问题或问题，请[阅读在线文档](https://htmlpreview.github.io/?https://github.com/Klocman/Bulk-Crap-Uninstaller/blob/master/doc/BCU_manual.html)（所有版本都包含帮助文件）。如果没有找到您问题的答案，请随时[提交新问题](https://github.com/Klocman/Bulk-Crap-Uninstaller/issues/new)。

## 下载
您可以从发布页面获取最新版本。或者，您也可以从以下任一站点下载：
- [从 dAppCDN 下载](https://dappcdn.com/download/utilities/bulk-crap-uninstaller)
- [从 FossHub 下载](https://www.fosshub.com/Bulk-Crap-Uninstaller.html)
- [从 SourceForge 下载](https://sourceforge.net/projects/bulk-crap-uninstaller/)

#### 不同版本有什么区别？
- 安装版（Setup）- 将 BCU 作为普通应用程序安装。如果您的系统缺少所需的 .NET 运行时，它也会自动安装。
- 便携版（Portable）- 独立版本，不需要 .NET 运行时即可运行。它包含运行时，这就是文件大小如此之大的原因。
- net 版 - 独立便携版本，需要安装 .NET 运行时。文件大小比完整便携版小得多。

#### 每日构建版
如果您想第一时间获得最新功能和修复，可以从 [操作页面](https://github.com/Klocman/Bulk-Crap-Uninstaller/actions/workflows/ci.yaml) 下载每日构建版。

## 系统要求
#### BCUninstaller v6
- 最低支持操作系统：Windows 10（可能在 Windows 7 上运行）
- 要求：.NET 8 桌面运行时（便携版不需要）

要获取此版本，请从下方链接下载最新版本。

_*注意：由于支持的系统都没有 x86 版本，v6 版本不再包含 x86 构建。如果需要，您仍然可以自己编译，或者使用 AnyCPU 构建。_

#### BCUninstaller v5
- 最低支持操作系统：Windows 7 SP1 并安装所有平台更新（KB2670838、KB2533623 等）
- 要求：.NET 6 桌面运行时（便携版不需要）

如果启动时出现 DLL 错误，请尝试运行 Windows 更新。如果出现框架错误，请手动或通过 Windows 更新安装 .NET 6。

要获取此版本，请下载 [最新的 5.x 版本](https://github.com/Klocman/Bulk-Crap-Uninstaller/releases/tag/v5.9)。

_*注意：便携版不需要安装 .NET 6 运行时，因为它已经包含在内（这就是便携版如此之大的原因）。_

#### BCUninstaller v1 - v4
- 最低支持操作系统：Windows XP（在更高版本中 XP 支持可能不稳定）
- 要求：.Net Framework 4.5（某些版本可以在 .Net Framework 3.5 上运行，但功能会减少）

确保您已安装 .Net Framework 4.5 并为您的系统安装了所有可用更新（XP 默认不安装它）。

要获取此版本，请编译 [旧版 4.x 分支](https://github.com/Klocman/Bulk-Crap-Uninstaller/tree/legacy-4.x) 或下载 [最新的 4.x 版本](https://github.com/Klocman/Bulk-Crap-Uninstaller/releases/tag/v4.16)。

## 我能帮上什么忙？
请查看 [贡献指南](https://github.com/BCUninstaller/Bulk-Crap-Uninstaller/blob/master/CONTRIBUTING.md)！

## 编译
开发在 Visual Studio 2022 上进行。只要安装了必要的 VS 功能，解决方案应该可以直接加载和构建，无需额外操作。
安装程序使用 InnoSetup v6.4 编译。要发布版本，您必须首先运行 `publish.bat` 脚本。

## 截图
![预览](https://bcuninstaller.github.io/Bulk-Crap-Uninstaller/assets/1.png)
![预览](https://bcuninstaller.github.io/Bulk-Crap-Uninstaller/assets/4.png)
