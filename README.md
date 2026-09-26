# Algora Bounty Setup Guide / Algora 赏金配置指南

This repository explains how to install, configure, and use the **Algora** bounty bot on GitHub repositories to reward open-source contributors.

本项目为你提供在 GitHub 仓库中配置和使用 **Algora** 赏金机器人的完整指南。

---

## 1. Quick Setup / 快速安装

1. **Sign in / 登录平台:** Visit [algora.io](https://algora.io) and link your GitHub account.
2. **Install Bot / 安装机器人:** Grant repository permissions to the official `@algora-pbc` bot via GitHub Apps.
3. **Connect Payouts / 绑定支付:** Add your payment method (Stripe / Credit Card / Crypto) in your Algora organization settings.

---

## 2. Managing Bounties (Maintainer Commands) / 维护者常用命令

Place these commands directly in an issue comment:

| Command / 命令 | Description / 作用 | Example / 示例 |
|---|---|---|
| `/bounty $XX` | Creates and funds a bounty on the issue / 在该 Issue 上创建并托管赏金 | `/bounty $50` |
| `/tip $XX @user` | Direct tip to a contributor / 直接打赏指定贡献者 | `/tip $20 @contributor` |
| `/cancel` | Cancels an uncompleted bounty / 撤销尚未完成的赏金 | `/cancel` |

---

## 3. Claiming Bounties (Contributor Workflow) / 贡献者认领规则

1. Fork the repository and fix the issue in a local branch.
2. Open a Pull Request referencing the issue:
   ```markdown
   Fixes #1
   @algora-pbc /claim #1
   ```
3. When the maintainer clicks **Merge pull request**, Algora automatically transfers the bounty reward to the contributor account.

---

> Generated to resolve Issue #1: Complete operational overview of Algora workflows.
