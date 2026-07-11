---
dg-publish: true
tags:
  - AI
  - 技术趋势
created: 2026-07-10
---

# AI技术趋势

GitHub 于 2026 年 2 月发布了 **GitHub Agentic Workflows** 技术预览版，这标志着 [[人工智能]] 在软件开发流程中的深度集成迈出了关键一步。该功能由 GitHub Next、Microsoft Research 和 Azure Core Upstream 联合打造，将 [[大语言模型]] 驱动的编码代理引入 GitHub Actions，实现了以自然语言描述意图、由 AI 代理自动执行的全新自动化范式。

GitHub Agentic Workflows 的核心理念是"**意图驱动的仓库自动化**"：开发者用纯 Markdown 描述期望的结果，系统通过编码代理（如 Copilot CLI、Claude Code、OpenAI Codex）在 GitHub Actions 中执行。它提出了"**Continuous AI**"概念——将 [[人工智能]] 集成到软件开发生命周期中，类似于 CI/CD 实践对持续集成和部署的增强。典型应用场景包括：持续分流（自动标记和路由 Issue）、持续文档（保持文档与代码同步）、持续代码简化（识别改进并提交 PR）、持续测试改进（评估覆盖率并补充测试）、持续质量维护（调查 CI 失败并提修复建议）以及持续报告（定期生成仓库健康报告）。

在安全方面，GitHub 采用了**纵深防御架构**：工作流默认只读权限，写操作需通过"安全输出"（safe outputs）显式审批；同时提供沙箱执行、工具白名单和网络隔离等防护机制，确保代理在受控边界内运行。所有 PR 不会自动合并，始终需要人类审查批准。

## 关键要点
- GitHub Agentic Workflows 将编码代理与 GitHub Actions 深度整合，用 Markdown 编写自动化意图，由 AI 代理执行
- 提出 Continuous AI 概念，涵盖持续分流、持续文档、持续代码简化、持续测试改进等六大应用场景
- 采用纵深防御安全架构：默认只读、安全输出审批、沙箱隔离，确保 [[人工智能]] 代理在受控边界内运行
- 支持多种编码代理引擎（Copilot CLI、Claude Code、OpenAI Codex），可与现有 CI/CD 流程互补
- 强调人类始终在环路中，PR 不自动合并，代理工作结果需人工审查

## 相关链接
- [[知识体系构建]]
