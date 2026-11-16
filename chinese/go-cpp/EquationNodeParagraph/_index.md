---
title: "EquationNodeParagraph 类"
linktitle: "EquationNodeParagraph"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "EquationNodeParagraph 类。封装在 Go 中表示 equationnodeparagraph 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/equationnodeparagraph/
---

## EquationNodeParagraph class

此类指定包含一个或多个 MathEquationNode(OMath) 元素的数学段落。

```go

type EquationNodeParagraph struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewEquationNodeParagraph](./newequationnodeparagraph/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetJustification](./getjustification/) | 此属性指定数学段落的对齐方式（同一段落内相邻方程的系列）。数学段落可以左对齐、右对齐、居中或整体居中。默认情况下，数学段落为整体居中。这意味着方程之间可以相互对齐，但整个方程组整体居中。 |
| [SetJustification](./setjustification/) | 此属性指定数学段落的对齐方式（同一段落内相邻方程的系列）。数学段落可以左对齐、右对齐、居中或整体居中。默认情况下，数学段落为整体居中。这意味着方程之间可以相互对齐，但整个方程组整体居中。 |
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
| [EquationNodeParagraph_CreateNode](./equationnodeparagraph_createnode/) | 创建指定类型的节点。 |
