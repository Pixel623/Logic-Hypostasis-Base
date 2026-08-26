# Logic‑Hypostasis‑Base(LHB)：逻辑位格基底元语法框架
> A Metagrammar Framework Complementing Classical Formal Logic

[![License: MIT](https://img.shields.io/badge/license‑MIT‑blue.svg)](LICENSE)

## 项目简介
Logic‑Hypostasis‑Base（LHB，逻辑位格基底）是一套**补充性元逻辑/元语法理论框架**，并不替代经典命题‑谓词演算，而是在其上层新增元语法校验层，专门处理位格漂移、论域边界僭越、主客体层级坍缩、范畴混淆等元语法层面产生的逻辑缺陷。

该框架为东西方经典悖论（说谎者悖论、全能悖论、白马非马等）提供统一形式诊断工具。本仓库为配套学术论文的理论存档仓库，**目前以理论规范、公理体系、案例文本为主，完整自动化符号演算引擎属于未来待实现工作**。

配套学术论文：
> 《位格与边界：一种补足经典形式逻辑的元语法框架及悖论统一诊断研究》
> 投稿期刊：《逻辑学研究》（Studies in Logic，CSSCI集刊）

> ⚠️重要声明
> 1. LHB **兼容经典形式逻辑对象层推演，不否定、不推翻现有数理逻辑体系**；
> 2. 本框架目标是**诊断悖论生成的元语法根源，不是彻底消解悖论**；
> 3. 仓库内大模型Prompt演示仅属于下游工程示例，不属于论文核心理论创新；
> 4. 当前缺陷张量`strength`强度参数为启发式赋值，完整公理化属于后续研究方向。

## 核心概念（四大元语法原语）
1. **本体 $\mathcal{L}$**：意义基底，无边界、无位格，为概念与命题提供存在基础。
2. **视野 $\mathcal{H}$**：言说主体可讨论的语义域，随主体位格动态变化。
3. **位格 $\star^n$**：言说主体的层级身份，决定合法言说权限与视野范围；$n$代表层级。
4. **边界 $\partial_\alpha$**：视野的约束阈值，主体不能未经许可僭越自身边界。

## 核心形式构件
1. **论辩四元组模型**
$$U \mapsto (\lceil S,\lceil B,\lceil r,\lceil t)$$
- $\lceil S$：主体；$\lceil B$：客体；$\lceil r$：关系；$\lceil t$：变换（视角切换、概念重定义等）

2. **缺陷张量 $\mathfrak{D}$**
$$\mathfrak{D} = [\text{type},\ \text{level},\ \text{truth\_value},\ \text{strength}]$$
用于结构化标记元语法缺陷：缺陷类型、缺陷层级、真值状态、缺陷破坏强度。

3. **两条基础公理 AX‑1，AX‑2 + 五条衍生定理 TH‑1~TH‑5**
> 公理与定理完整文本见：`docs/axioms_theorems.md`

## 案例库
案例均来自论文实证分析，每例包含四元组拆解、缺陷张量输出、与传统方案对比。
- `cases/liar_paradox.md` 说谎者悖论：主‑客体位格坍缩
- `cases/omnipotence_paradox.md` 全能悖论：跨位格边界越界
- `cases/white_horse.md` 白马非马：概念位格漂移与范畴混淆

## 仓库目录结构
```
├── docs/
│   ├── lhb_spec.md          # LHB完整理论规范文档
│   ├── axioms_theorems.md   # 公理、定理完整文本与动机说明
│   ├── glossary.md          # 术语对照表（中文‑英文‑符号）
│   └── journal‑submission/  # 论文相关材料（匿名稿件副本、参考文献）
├── cases/                   # 悖论案例库
├── demos/
│   └── llm‑prompt‑demo.md   # ⚠️下游演示：大模型诊断Prompt（非理论核心）
├── LICENSE
└── README.md
```

## 现状与未来工作
### 当前状态
✅ 完整元语法理论体系、公理定理、三大经典悖论案例、术语规范。
❌ **尚未实现自动化符号演算引擎，无可执行程序**。

### 未来研究方向
1. 完成缺陷张量`strength`维度全公理化；
2. 扩充案例库，覆盖更多哲学谬误、日常论辩文本；
3. 开发符号演算原型，实现元语法缺陷自动校验；
4. 探索在AI论证分析领域的下游应用。

## 引用
如果你在研究中参考本框架，请引用配套期刊论文（待正式出版）：
```bibtex
@article{lhb2026,
  title={位格与边界：一种补足经典形式逻辑的元语法框架及悖论统一诊断研究},
  journal={逻辑学研究},
  author={Anonymous},
  year={2026}
}
```

> 开源协议：MIT License，可自由阅读、引用、二次非商业/商业使用，保留版权声明。
```
