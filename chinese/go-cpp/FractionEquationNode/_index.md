---
title: "FractionEquationNode 类"
linktitle: "FractionEquationNode"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "FractionEquationNode 类。封装了在 Go 中表示 fractionequationnode 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/fractionequationnode/
---

## FractionEquationNode class

此类指定分数方程，由分子和分母通过分数线分隔组成。分数线可以是水平的或对角的，取决于分数属性。分数方程也用于表示堆叠函数，即将一个元素置于另一个元素之上且不使用分数线。

```go

type FractionEquationNode struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewFractionEquationNode](./newfractionequationnode/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetFractionType](./getfractiontype/) | 这指定了分数的类型；默认值为 'Bar'。 |
| [SetFractionType](./setfractiontype/) | 这指定了分数的类型；默认值为 'Bar'。 |
| [Equals](./equals/) | 确定当前方程节点是否等于指定的节点 |
| [GetStartIndex](./getstartindex/) | 获取字符的起始索引。 |
| [GetLength](./getlength/) | 获取字符的长度。 |
| [GetFont](./getfont/) | 返回此对象的字体。 |
| [SetWordArtStyle](./setwordartstyle/) | 设置预设的 WordArt 样式。 |
| [GetTextOptions](./gettextoptions/) | 返回文本选项。 |
| [GetType](./gettype/) | 获取文本节点的类型。 |
| [GetParentNode](./getparentnode/) | 指定当前节点的父节点 |
| [SetParentNode](./setparentnode/) | 指定当前节点的父节点 |
| [ToLaTeX](./tolatex/) | 将此等式转换为 LaTeX 表达式。 |
| [ToMathML](./tomathml/) | 将此等式转换为 MathML 表达式。 |
| [AddChild_EquationNodeType](./addchild_equationnodetype/) | 在当前节点的子节点列表末尾插入指定类型的节点。 |
| [InsertChild](./insertchild/) | 在当前节点的子节点列表中指定的索引位置插入指定类型的节点。 |
| [InsertAfter](./insertafter/) | 在当前节点之后插入指定的节点。 |
| [InsertBefore](./insertbefore/) | 在当前节点之前插入指定的节点。 |
| [GetChild](./getchild/) | 返回当前节点子节点中指定索引处的节点。 |
| [Remove](./remove/) | 从父节点中移除自身。 |
| [RemoveChild_EquationNode](./removechild_equationnode/) | 从当前节点的子节点中移除指定的节点。 |
| [RemoveAllChildren](./removeallchildren/) | 移除当前节点的所有子节点。 |
| [GetEquationType](./getequationtype/) | 获取当前节点的方程类型 |
| [FractionEquationNode_CreateNode](./fractionequationnode_createnode/) | 创建指定类型的节点。 |
