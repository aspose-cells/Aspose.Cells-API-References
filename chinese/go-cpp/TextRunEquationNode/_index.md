---
title: "TextRunEquationNode 类"
linktitle: "TextRunEquationNode"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "TextRunEquationNode 类。封装在 Go 中表示 textrunequationnode 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/textrunequationnode/
---

## TextRunEquationNode class

方程节点中的此类用于存储方程的实际内容（数学文本序列）。通常每个字符对应一个节点对象。

```go

type TextRunEquationNode struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewTextRunEquationNode](./newtextrunequationnode/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetText](./gettext/) | 设置文本节点的内容（通常每个字符对应一个节点对象）。 |
| [SetText](./settext/) | 设置文本节点的内容（通常每个字符对应一个节点对象）。 |
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
| [TextRunEquationNode_CreateNode](./textrunequationnode_createnode/) | 创建指定类型的节点。 |
