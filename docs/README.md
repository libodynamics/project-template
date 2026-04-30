<!-- Copyright The Project Template Contributors -->

# docs/

本目录保存项目文档。

## 目录结构

```text
docs/
  README.md
  conventions.md
  git.md
  SAD.md             # 可选，当前软件架构
  SDD.md             # 可选，当前软件设计
  adr/
    README.md
    template.md
  rfcs/
    README.md
    template.md
  specs/
    template.md
  plans/
    template.md
  templates/
    README.md
    sad.md
    sdd.md
    local-AGENTS.md
    hardware-design.md
    supplier-record.md
    sop.md
  screenshots/
  hardware/       # 可选
  production/     # 可选
  suppliers/      # 可选
  sop/            # 可选
```

## 文档类型指南

| 需求 | 应写文档 |
|------|----------|
| 描述当前软件架构、运行时/部署视图、架构约束和质量属性 | `docs/SAD.md` |
| 描述当前系统或子系统设计、接口、数据模型、状态机和算法 | `docs/SDD.md` |
| 记录已经做出的架构决策 | `docs/adr/` |
| 在决策前讨论较大的设计方向 | `docs/rfcs/` |
| 描述功能或子系统设计 | `docs/specs/` |
| 跟踪实施步骤 | `docs/plans/` |
| 创建局部模块规则、硬件设计、供应商记录或 SOP | `docs/templates/` |
| 记录语言、文档、测试、安全等长期约定 | `docs/conventions.md` |
| 记录 Git 工作流和 commit 规范 | `docs/git.md` |
| 说明安装、编译、运行、测试命令 | 根目录 `README.md` |
| 定义项目级规则 | 根目录 `AGENTS.md` |

图表优先使用 Mermaid 或 PlantUML。涉及硬件拓扑、生产流程、供应商边界或 SOP 的文档，应同时保留可审查的文字说明和图表。

SAD/SDD 与 ADR/RFC/Spec/Plan 的边界：

- SAD 说明“当前架构是什么”，应引用 ADR 解释关键决策来源。
- SDD 说明“当前设计如何落地”，可按子系统拆分，也可作为项目级设计文档。
- ADR 记录“为什么做出这个决策”，不替代 SAD/SDD 的当前状态说明。
- RFC 记录决策前的设计空间探索。
- Spec 记录某个功能或子系统的设计输入；设计稳定后应同步到 SDD 或在 SDD 中链接。
- Plan 记录执行步骤和验证，不替代设计文档。
