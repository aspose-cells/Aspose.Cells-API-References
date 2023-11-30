﻿---
title: Aspose::Cells::Drawing::Equations::DelimiterEquationNode class
linktitle: DelimiterEquationNode
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Equations::DelimiterEquationNode class. This class specifies the delimiter equation, consisting of opening and closing delimiters (such as parentheses, braces, brackets, and vertical bars), and a component contained inside. The delimiter may have more than one component, with a designated separator character between each component in C++.'
type: docs
weight: 500
url: /cpp/aspose.cells.drawing.equations/delimiterequationnode/
---
## DelimiterEquationNode class


This class specifies the delimiter equation, consisting of opening and closing delimiters (such as parentheses, braces, brackets, and vertical bars), and a component contained inside. The delimiter may have more than one component, with a designated separator character between each component.

```cpp
class DelimiterEquationNode : public Aspose::Cells::Drawing::Equations::EquationNode
```

## Methods

| Method | Description |
| --- | --- |
| [AddChild(EquationNodeType equationType)](../equationnode/addchild/) | Insert a node of the specified type at the end of the child node list of the current node. |
| [AddChild(const EquationNode\& node)](../equationnode/addchild/) | Inserts the specified node at the end of the current node's list of child nodes. |
| static [CreateNode(EquationNodeType equationType, const Workbook\& workbook, const EquationNode\& parent)](../equationnode/createnode/) | Create a node of the specified type. |
| [DelimiterEquationNode(DelimiterEquationNode_Impl* impl)](./delimiterequationnode/) | Constructs from an implementation object. |
| [DelimiterEquationNode(const DelimiterEquationNode\& src)](./delimiterequationnode/) | Copy constructor. |
| [DelimiterEquationNode(const EquationNode\& src)](./delimiterequationnode/) | Constructs from a parent object. |
| [EquationNode(EquationNode_Impl* impl)](../equationnode/equationnode/) | Constructs from an implementation object. |
| [EquationNode(const EquationNode\& src)](../equationnode/equationnode/) | Copy constructor. |
| [EquationNode(const FontSetting\& src)](../equationnode/equationnode/) | Constructs from a parent object. |
| [FontSetting(int32_t startIndex, int32_t length, const WorksheetCollection\& sheets)](../../aspose.cells/fontsetting/fontsetting/) |  |
| [FontSetting(FontSetting_Impl* impl)](../../aspose.cells/fontsetting/fontsetting/) | Constructs from an implementation object. |
| [FontSetting(const FontSetting\& src)](../../aspose.cells/fontsetting/fontsetting/) | Copy constructor. |
| [GetBeginChar()](./getbeginchar/) | Delimiter beginning character. |
| [GetChild(int32_t index)](../equationnode/getchild/) | Returns the node at the specified index among the children of the current node. |
| [GetDelimiterShape()](./getdelimitershape/) | Specifies the shape of delimiters in the delimiter object. |
| [GetEndChar()](./getendchar/) | Delimiter ending character. |
| [GetEquationType()](../equationnode/getequationtype/) | Get the equation type of the current node. |
| [GetFont()](../../aspose.cells/fontsetting/getfont/) | Returns the font of this object. |
| [GetLength()](../../aspose.cells/fontsetting/getlength/) | Gets the length of the characters. |
| [GetNaryGrow()](./getnarygrow/) | This property specifies the growth property of the delimiter at the document level. When off, the delimiter will not grow to match the size of its component height. When enabled, the delimiter grows vertically to match its component height. |
| [GetParentNode()](../equationnode/getparentnode/) | Specifies the parent node of the current node. |
| [GetSeparatorChar()](./getseparatorchar/) | Delimiter separator character. |
| [GetStartIndex()](../../aspose.cells/fontsetting/getstartindex/) | Gets the start index of the characters. |
| [GetTextOptions()](../../aspose.cells/fontsetting/gettextoptions/) | Returns the text options. |
| [GetType()](../equationnode/gettype/) | Represents the type of the node. |
| [InsertAfter(EquationNodeType equationType)](../equationnode/insertafter/) | Inserts the specified node after the current node. |
| [InsertBefore(EquationNodeType equationType)](../equationnode/insertbefore/) | Inserts the specified node before the current node. |
| [InsertChild(int32_t index, EquationNodeType equationType)](../equationnode/insertchild/) | Inserts a node of the specified type at the specified index position in the current node's child node list. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const DelimiterEquationNode\& src)](./operator_asm/) | operator= |
| [operator=(const EquationNode\& src)](../equationnode/operator_asm/) | operator= |
| [operator=(const FontSetting\& src)](../../aspose.cells/fontsetting/operator_asm/) | operator= |
| [Remove()](../equationnode/remove/) | Removes itself from the parent. |
| [RemoveAllChildren()](../equationnode/removeallchildren/) | Removes all the child nodes of the current node. |
| [RemoveChild(const EquationNode\& node)](../equationnode/removechild/) | Removes the specified node from the current node's children. |
| [RemoveChild(int32_t index)](../equationnode/removechild/) | Removes the node at the specified index from the current node's children. |
| [SetBeginChar(const U16String\& value)](./setbeginchar/) | Delimiter beginning character. |
| [SetBeginChar(const char16_t* value)](./setbeginchar/) | Delimiter beginning character. |
| [SetDelimiterShape(EquationDelimiterShapeType value)](./setdelimitershape/) | Specifies the shape of delimiters in the delimiter object. |
| [SetEndChar(const U16String\& value)](./setendchar/) | Delimiter ending character. |
| [SetEndChar(const char16_t* value)](./setendchar/) | Delimiter ending character. |
| [SetNaryGrow(bool value)](./setnarygrow/) | This property specifies the growth property of the delimiter at the document level. When off, the delimiter will not grow to match the size of its component height. When enabled, the delimiter grows vertically to match its component height. |
| [SetParentNode(const EquationNode\& value)](../equationnode/setparentnode/) | Specifies the parent node of the current node. |
| [SetSeparatorChar(const U16String\& value)](./setseparatorchar/) | Delimiter separator character. |
| [SetSeparatorChar(const char16_t* value)](./setseparatorchar/) | Delimiter separator character. |
| [SetWordArtStyle(PresetWordArtStyle style)](../../aspose.cells/fontsetting/setwordartstyle/) | Sets the preset WordArt style. |
| [~DelimiterEquationNode()](./~delimiterequationnode/) | Destructor. |
| [~EquationNode()](../equationnode/~equationnode/) | Destructor. |
| [~FontSetting()](../../aspose.cells/fontsetting/~fontsetting/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also

* Class [EquationNode](../equationnode/)
* Namespace [Aspose::Cells::Drawing::Equations](../)
* Library [Aspose.Cells for C++](../../)
