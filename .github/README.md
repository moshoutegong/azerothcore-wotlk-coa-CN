# ![AzerothCore 标志](https://raw.githubusercontent.com/azerothcore/azerothcore.github.io/master/images/logo-github.png) AzerothCore

[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)
[![CodeFactor](https://www.codefactor.io/repository/github/azerothcore/azerothcore-wotlk/badge)](https://www.codefactor.io/repository/github/azerothcore/azerothcore-wotlk)
[![Discord](https://img.shields.io/discord/217589275766685707?logo=discord&logoColor=white)](https://discord.gg/gkt4y2x "Discord 社区")

## 构建状态

以下徽章显示上游 AzerothCore 的构建状态。

[![nopch-build](https://github.com/azerothcore/azerothcore-wotlk/actions/workflows/core-build-nopch.yml/badge.svg?branch=master)](https://github.com/azerothcore/azerothcore-wotlk/actions/workflows/core-build-nopch.yml?query=branch%3Amaster)
[![pch-build](https://github.com/azerothcore/azerothcore-wotlk/actions/workflows/core-build-pch.yml/badge.svg?branch=master)](https://github.com/azerothcore/azerothcore-wotlk/actions/workflows/core-build-pch.yml?query=branch%3Amaster)
[![core-modules-build](https://github.com/azerothcore/azerothcore-wotlk/actions/workflows/core_modules_build.yml/badge.svg?branch=master)](https://github.com/azerothcore/azerothcore-wotlk/actions/workflows/core_modules_build.yml?query=branch%3Amaster)
[![windows-build](https://github.com/azerothcore/azerothcore-wotlk/actions/workflows/windows_build.yml/badge.svg?branch=master)](https://github.com/azerothcore/azerothcore-wotlk/actions/workflows/windows_build.yml?query=branch%3Amaster)
[![macos-build](https://github.com/azerothcore/azerothcore-wotlk/actions/workflows/macos_build.yml/badge.svg?branch=master)](https://github.com/azerothcore/azerothcore-wotlk/actions/workflows/macos_build.yml?query=branch%3Amaster)
[![docker-build](https://github.com/azerothcore/azerothcore-wotlk/actions/workflows/docker_build.yml/badge.svg?branch=master)](https://github.com/azerothcore/azerothcore-wotlk/actions/workflows/docker_build.yml?query=branch%3Amaster)
[![tools-build](https://github.com/azerothcore/azerothcore-wotlk/actions/workflows/tools_build.yml/badge.svg?branch=master)](https://github.com/azerothcore/azerothcore-wotlk/actions/workflows/tools_build.yml?query=branch%3Amaster)
[![dashboard-ci](https://github.com/azerothcore/azerothcore-wotlk/actions/workflows/dashboard-ci.yml/badge.svg?branch=master)](https://github.com/azerothcore/azerothcore-wotlk/actions/workflows/dashboard-ci.yml?query=branch%3Amaster)

## 项目简介

AzerothCore 是一套用于搭建大型多人在线角色扮演游戏（MMORPG）的开源服务端程序和框架。
项目以《魔兽世界》为基础，致力于还原《巫妖王之怒》3.3.5a 版本的游戏体验。

项目的早期代码源自 MaNGOS、TrinityCore 和 SunwellCore。经过持续开发，AzerothCore 改善了服务端稳定性、游戏机制和模块化程度，
也逐渐发展成由众多开发者和贡献者共同维护的社区项目。它使用 C++ 编写，可作为搭建模拟《魔兽世界》官方服务端行为的私有服务器的基础。

## 项目理念

我们的首要目标是打造可实际游玩的服务端，让各项游戏功能正常运转。

* **稳定性**。所有变更须通过持续集成（CI）检查，才能合并到上游 `master` 分支。

* **还原官方体验**。我们力求让游戏内容贴近暴雪原版，并对修复的准确性有较高要求。

* **易于定制**。通过[模块](#模块)即可定制游戏体验。

* **社区驱动**。开发者、贡献者和用户通过论坛、Discord 等平台协作、分享经验并互相提供支持。

### 模块

AzerothCore 采用模块化设计，开发者可以扩展和定制游戏，添加自定义功能、内容和玩法。

社区已开发了许多模块，可在[模块目录](https://www.azerothcore.org/catalogue.html#/)中查找。

## 安装

在这个 CoA（Conquest of Azeroth）分支中，当 `Updates.AutoSetup` 创建空白世界数据库时，
`worldserver` 和 `dbimport` 会从[世界数据库包](../apps/coa-world/README.md)导入初始数据。

详细步骤请参阅 [AzerothCore 安装指南](http://www.azerothcore.org/wiki/installation)。

## 参与贡献

如果你想了解《魔兽世界》服务端的运行原理、MMORPG 的结构或游戏服务端模拟器的开发方式，
也可以通过 AzerothCore 学习和练习 C++ 与 SQL。

有意参与项目的开发者可以查阅 [Wiki 贡献指南](https://www.azerothcore.org/wiki/contribute)。

参与前也建议阅读[贡献者行为准则](https://github.com/azerothcore/azerothcore-wotlk/blob/master/.github/CODE_OF_CONDUCT.md)。

欢迎加入 [Discord 服务器](https://discord.gg/gkt4y2x)。

🤖 如果你使用 AI 智能体参与 AzerothCore 开发，请先阅读 [AI 智能体开发指南](https://www.azerothcore.org/wiki/agentic-engineering)。
本仓库的智能体规则见 [AGENTS.md](../AGENTS.md) 和 [.agents/rules/](../.agents/rules/)。
各类任务的操作指南位于 [.agents/docs/](../.agents/docs/)，配置方法见 [.agents/README.md](../.agents/README.md)。

欢迎点击「⭐ Star」，让更多 GitHub 用户发现这个项目。

## 作者与贡献者

本项目于 2016 年基于 SunwellCore 创建。由于 SunwellCore 发布时未附带 Git 历史，
项目的 Git 记录无法完整反映 2016 年以前的贡献。

详情请参阅 [AUTHORS 文件](https://github.com/azerothcore/azerothcore-wotlk/blob/master/AUTHORS)。

## 相关链接

- [Doxygen 文档](https://www.azerothcore.org/pages/doxygen/index.html)
- [官方网站](http://www.azerothcore.org/)
- [AzerothCore 资源目录](http://www.azerothcore.org/catalogue.html "AzerothCore 模块、工具及其他资源")
- [Discord 社区](https://discord.gg/gkt4y2x)
- [Wiki](http://www.azerothcore.org/wiki "由 AzerothCore 创始人开发，便于查阅")
- [GitHub 讨论区](https://github.com/azerothcore/azerothcore-wotlk/discussions/)
- [Facebook 主页](https://www.facebook.com/AzerothCore/)
- [LinkedIn 主页](https://www.linkedin.com/company/azerothcore/)

## 许可证

AzerothCore 源代码依据 [GNU GPL v2](https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html) 发布。

AzerothCore 属于独立的社区项目，与《魔兽世界》及暴雪娱乐均无隶属关系，也未获得其认可。AzerothCore 在任何情况下均不赞助或支持非法公开服务器。
本项目可供测试和学习。使用本项目运行非法公开服务器属于使用者的个人决定。

## 特别鸣谢

[JetBrains](https://www.jetbrains.com/?from=AzerothCore) 为 AzerothCore 开发者免费提供[开源项目许可证](https://www.jetbrains.com/community/opensource/)。

[![JetBrains 标志](https://resources.jetbrains.com/storage/products/company/brand/logos/jetbrains.svg)](https://jb.gg/OpenSourceSupport)
