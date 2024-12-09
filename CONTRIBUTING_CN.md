# 贡献指南

[English](./CONTRIBUTING.md) | 中文

感谢您考虑为 JLU Software 做出贡献！本文档概述了参与我们项目的指南。

## 目录

- [贡献指南](#贡献指南)
  - [目录](#目录)
  - [快速开始](#快速开始)
  - [开发流程](#开发流程)
  - [Pull Request 规范](#pull-request-规范)
  - [代码规范](#代码规范)
    - [Python](#python)
    - [C++](#c)
    - [JavaScript/TypeScript](#javascripttypescript)
  - [提交信息规范](#提交信息规范)
  - [文档规范](#文档规范)
  - [测试规范](#测试规范)
  - [Issue 指南](#issue-指南)
    - [Bug 报告](#bug-报告)
    - [功能请求](#功能请求)
  - [审查流程](#审查流程)
  - [有问题？](#有问题)

## 快速开始

1. Fork 仓库
2. 克隆你的 fork：

   ```bash
   git clone https://github.com/your-username/repository-name.git
   ```

3. 添加上游仓库：

   ```bash
   git remote add upstream https://github.com/jlu-software/repository-name.git
   ```

4. 为你的功能/修复创建新分支：

   ```bash
   git checkout -b feature/your-feature-name
   ```

## 开发流程

1. 保持分支更新：

   ```bash
   git pull upstream main
   ```

2. 以小而逻辑清晰的单位提交更改
3. 为更改编写测试
4. 根据需要更新文档
5. 提交前运行本地测试
6. 推送更改到你的 fork
7. 创建 Pull Request

## Pull Request 规范

- 完整填写 PR 模板
- 关联相关的 issues
- 对于 UI 更改，包含截图/GIF
- 更新相关文档
- 添加/更新测试
- 确保所有 CI 检查通过
- 请求相关团队成员审查

## 代码规范

### Python

- 遵循 PEP 8 风格指南
- 使用类型提示标注函数参数和返回值
- 使用文档字符串记录函数和类
- 最大行长度：88 字符
- 使用 black 进行代码格式化

示例：

```python
def calculate_distance(point_a: Tuple[float, float], point_b: Tuple[float, float]) -> float:
    """计算两点间的欧几里得距离。

    参数:
        point_a: 第一个点的 (x, y) 坐标元组
        point_b: 第二个点的 (x, y) 坐标元组

    返回:
        表示两点间距离的浮点数
    """
    return math.sqrt((point_b[0] - point_a[0])**2 + (point_b[1] - point_a[1])**2)
```

### C++

- 遵循 Google C++ 风格指南
- 使用现代 C++ 特性（C++14 或更新）
- 使用 Doxygen 风格记录类和函数
- 最大行长度：100 字符
- 使用 clang-format 进行代码格式化

### JavaScript/TypeScript

- 遵循 Airbnb JavaScript 风格指南
- 使用 ESLint 和 Prettier 进行格式化
- 新功能使用 TypeScript
- 最大行长度：80 字符

## 提交信息规范

遵循约定式提交规范：

```plaintext
<类型>(<范围>): <描述>

[可选的正文]

[可选的脚注]
```

类型：

- feat: 新功能
- fix: 修复 bug
- docs: 文档更改
- style: 代码风格更改（格式化等）
- refactor: 代码重构
- test: 添加或更新测试
- chore: 维护任务

示例：

```plaintext
feat(navigation): 添加路径规划算法

实现了 A* 算法用于机器人路径规划。
添加了单元测试和文档。

Closes #123
```

## 文档规范

- 记录所有公共 API
- 保持 README.md 更新
- 为复杂算法添加注释
- 包含使用示例
- 记录设置和部署步骤

## 测试规范

- 为新功能编写单元测试
- 保持测试覆盖率在 80% 以上
- 包含必要的集成测试
- 测试边界情况
- 记录测试场景

## Issue 指南

创建 issue 前：

1. 搜索现有 issues
2. 使用 issue 模板
3. 提供清晰的复现步骤
4. 包含系统/环境详情
5. 添加相关标签

### Bug 报告

- 描述预期与实际行为
- 包含复现步骤
- 附加截图/日志（如适用）
- 说明环境详情

### 功能请求

- 清晰描述要解决的问题
- 建议可能的解决方案
- 说明好处
- 考虑潜在的缺点

## 审查流程

1. 所有更改都需要代码审查
2. 更改必须通过所有 CI 检查
3. 必须更新文档
4. 测试必须通过
5. 必须处理审查意见

## 有问题？

随时在以下渠道提问：

- GitHub Discussions
- 团队聊天频道
- 开发者会议

感谢您为 JLU Software 做出贡献！
