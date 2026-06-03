# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 项目概述

**myPets** — 宠物管理应用，使用 Java 21 + IntelliJ IDEA 开发。

## 开发环境

- **JDK**: 21
- **IDE**: IntelliJ IDEA（项目文件在 `.idea/` 目录）
- **构建系统**: Maven（`pom.xml`）

## 项目结构

```
myPets/
├── .idea/          # IntelliJ IDEA 配置
├── .gitignore      # Java 标准 gitignore（基于 BlueJ 模板）
├── CLAUDE.md       # 本文件
└── README.md       # 项目说明
```

当前项目尚处于初始化阶段，仅有骨架结构，暂无源代码和构建配置。

## Git 分支策略

- `master` — 主分支，稳定版本
- `dev` — 开发分支（当前活动分支），新功能在此开发

开发流程：在 `dev` 分支上开发，完成后合并到 `master`。

## 常见命令

```bash
# Maven 构建
mvn clean compile        # 编译
mvn clean test           # 运行测试
mvn clean package        # 打包 JAR
mvn clean install        # 安装到本地仓库

# 查看当前状态
git status

# 切换分支
git checkout dev         # 切到开发分支
git checkout master       # 切到主分支

# 合并 dev 到 master
git checkout master
git merge dev
```
