# Multiple Agent

Multiple Agent 是一个基于 Spring Boot 和 Spring AI 的多智能体系统项目。该项目旨在提供一个可扩展的 AI 代理架构，支持多种 AI 模型和向量存储，便于集成和部署。

## 目录

- [项目概述](#项目概述)
- [技术栈](#技术栈)
- [功能特性](#功能特性)
- [系统要求](#系统要求)
- [安装指南](#安装指南)
- [配置说明](#配置说明)
- [运行项目](#运行项目)
- [测试](#测试)
- [项目结构](#项目结构)
- [贡献](#贡献)
- [许可证](#许可证)

## 项目概述

Multiple Agent 是一个基于 Spring Boot 和 Spring AI 构建的多智能体系统，可用于对话系统、推荐系统、向量处理等 AI 相关功能。该项目提供了一个可扩展的架构，支持多种 AI 模型和向量数据库。

## 技术栈

- Java 21
- Spring Boot 3.5.5
- Spring AI 1.0.1
- Ollama AI 模型
- PgVector 向量存储
- Maven 构建工具

## 功能特性

- 基于 Spring Boot 的 Web 服务基础架构
- 集成 Spring AI，支持 Ollama 模型和 PgVector 向量存储
- 支持通过 Advisor 进行向量存储的语义检索
- 提供基础测试框架和模块
- 可扩展的多智能体交互系统

## 系统要求

- Java 21 或更高版本
- Maven 3.6 或更高版本
- Ollama 运行时环境
- PostgreSQL 数据库（带 PgVector 插件）

## 安装指南

1. 克隆项目代码：
   ```bash
   git clone <repository-url>
   ```

2. 进入项目目录：
   ```bash
   cd multiple-agent
   ```

3. 编译项目：
   ```bash
   mvn clean package
   ```

## 配置说明

项目配置文件位于 `src/main/resources/application.properties`。默认配置如下：

```properties
spring.application.name=multiple-agent
```

根据需要添加其他配置，例如数据库连接、AI 模型参数等。

## 运行项目

可以使用以下命令运行项目：

```bash
mvn spring-boot:run
```

或者使用编译后的 jar 包运行：

```bash
java -jar target/multiple-agent-0.0.1-SNAPSHOT.jar
```

## 测试

运行测试用例：

```bash
mvn test
```

## 项目结构

```
multiple-agent/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/splititor/multipleagent/
│   │   │       └── MultipleAgentApplication.java
│   │   └── resources/
│   │       └── application.properties
│   └── test/
│       └── java/
│           └── com/splititor/multipleagent/
│               └── MultipleAgentApplicationTests.java
├── pom.xml
└── README.md
```

## 贡献

欢迎提交 Issue 和 Pull Request 来改进项目。

## 许可证

该项目使用 Apache License 2.0 许可证。