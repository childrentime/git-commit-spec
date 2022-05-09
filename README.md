# Git Commit 指南

## 消息格式

每个提交消息都由一个标题、一个正文和一个页脚组成。标题具有特殊格式，包括类型、范围和主题：

```git
<type>(<scope>): <subject>
<BLANK LINE>
<body>
<BLANK LINE>
<footer>
```

标题是强制性的，标题的范围是可选的。

提交信息的任何一行不能超过 100 个字符！这使得消息在 GitHub 以及各种 git 工具中更易于阅读。

## 回溯

如果提交回溯了之前的提交，它应该以 `revert:` 开头，后面跟随回溯提交的标题。在正文中它应该说：`This reverts commit <hash>`。，其中 `hash` 是要恢复的提交的 SHA。

## 类型

必须是以下之一：

- feat：一个新的功能
- fix：一个bug修复
- docs：仅文档更改
- style：不影响代码含义的更改（空格、格式、缺少分号等）
- refactor：既不修复错误也不添加功能的代码更改
- perf：提高性能的代码更改
- test：添加缺失或纠正现有测试
- chore：对构建过程或辅助工具和库（例如文档生成）的更改

## 范围

范围可以是指定提交更改位置的任何内容。

当更改影响多个范围时，您可以使用 *。

## 主题

主题包含对更改的简洁描述：

- 使用进行时语气：“change”不是“changed”也不是“changes”
- 第一个字母不要大写
- 末尾没有点（.）

## 主体

就像在`主题`中一样，使用进行时语气：“change”不是“changed”也不是“changes”。主题应该包括修改的动机，并将其与以前的行为进行对比。

## 底部

填写当涉及到破坏性更改，或者关闭 `Github Issue` 的时候的信息

## 参考

1. [angular commit规范](https://docs.google.com/document/d/1QrDFcIiPjSLDn3EL15IJygNPiHORgU1_OOAqWjiDU5Y/edit#)
