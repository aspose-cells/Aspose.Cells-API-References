---
title: "NaryEquationNode 类"
linktitle: "NaryEquationNode"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "NaryEquationNode 类。封装在 Go 中表示 naryequationnode 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/naryequationnode/
---

## NaryEquationNode class

此类指定 n 元运算符方程，由 n 元运算符、基数（或操作数）以及可选的上界和下界组成。

```go

type NaryEquationNode struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewNaryEquationNode](./newnaryequationnode/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [IsHideSubscript](./ishidesubscript/) | 是否显示下界 |
| [SetIsHideSubscript](./setishidesubscript/) | 是否显示下界 |
| [IsHideSuperscript](./ishidesuperscript/) | 是否显示上界 |
| [SetIsHideSuperscript](./setishidesuperscript/) | 是否显示上界 |
| [GetLimitLocation](./getlimitlocation/) | 此属性指定 n 元运算符中极限的位置。极限可以位于 n 元运算符的上下居中，或仅位于运算符的右侧。 |
| [SetLimitLocation](./setlimitlocation/) | 此属性指定 n 元运算符中极限的位置。极限可以位于 n 元运算符的上下居中，或仅位于运算符的右侧。 |
| [GetNaryOperator](./getnaryoperator/) | 一个 n 元运算符，例如 "∑"。强烈建议使用属性 NaryOperatorType 来设置 n 元运算符。如果在已知类型中找不到所需字符，请使用此属性设置。 |
| [SetNaryOperator](./setnaryoperator/) | 一个 n 元运算符，例如 "∑"。强烈建议使用属性 NaryOperatorType 来设置 n 元运算符。如果在已知类型中找不到所需字符，请使用此属性设置。 |
| [GetNaryOperatorType](./getnaryoperatortype/) | 一个 n 元运算符，例如 "∑" |
| [SetNaryOperatorType](./setnaryoperatortype/) | 一个 n 元运算符，例如 "∑" |
| [GetNaryGrow](./getnarygrow/) | 此属性指定文档级别 n 元运算符的增长属性。关闭时，积分和求和等 n 元运算符不会随操作数高度的大小而增长。开启时，n 元运算符会垂直增长以匹配其操作数的高度。 |
| [SetNaryGrow](./setnarygrow/) | 此属性指定文档级别 n 元运算符的增长属性。关闭时，积分和求和等 n 元运算符不会随操作数高度的大小而增长。开启时，n 元运算符会垂直增长以匹配其操作数的高度。 |
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
| [NaryEquationNode_CreateNode](./naryequationnode_createnode/) | 创建指定类型的节点。 |
