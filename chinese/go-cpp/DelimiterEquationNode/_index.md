---
title: "DelimiterEquationNode 类"
linktitle: "DelimiterEquationNode"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "DelimiterEquationNode 类。封装了在 Go 中表示 delimiterequationnode 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/delimiterequationnode/
---

## DelimiterEquationNode class

此类指定分隔符方程，由起始和结束分隔符（例如括号、花括号、方括号和竖线）以及其中包含的组件组成。分隔符可以包含多个组件，每个组件之间使用指定的分隔字符。

```go

type DelimiterEquationNode struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewDelimiterEquationNode](./newdelimiterequationnode/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetBeginChar](./getbeginchar/) | 分隔符起始字符。 |
| [SetBeginChar](./setbeginchar/) | 分隔符起始字符。 |
| [GetEndChar](./getendchar/) | 分隔符结束字符。 |
| [SetEndChar](./setendchar/) | 分隔符结束字符。 |
| [GetNaryGrow](./getnarygrow/) | 指定分隔符是否应随公式高度自动展开和收缩。 |
| [SetNaryGrow](./setnarygrow/) | 指定分隔符是否应随公式高度自动展开和收缩。 |
| [GetSeparatorChar](./getseparatorchar/) | 分隔符分隔字符。 |
| [SetSeparatorChar](./setseparatorchar/) | 分隔符分隔字符。 |
| [GetDelimiterShape](./getdelimitershape/) | 指定分隔符对象中分隔符的形状。 |
| [SetDelimiterShape](./setdelimitershape/) | 指定分隔符对象中分隔符的形状。 |
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
| [DelimiterEquationNode_CreateNode](./delimiterequationnode_createnode/) | 创建指定类型的节点。 |
