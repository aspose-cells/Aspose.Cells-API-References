﻿---
title: Aspose::Cells::Drawing::Equations::AccentEquationNode class
linktitle: AccentEquationNode
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Equations::AccentEquationNode class. This class specifies an accent equation, consisting of a base component and a combining diacritic in C++.'
type: docs
weight: 100
url: /cpp/aspose.cells.drawing.equations/accentequationnode/
---
## AccentEquationNode class


This class specifies an accent equation, consisting of a base component and a combining diacritic.

```cpp
class AccentEquationNode : public Aspose::Cells::Drawing::Equations::EquationNode
```

## Methods

| Method | Description |
| --- | --- |
| [AccentEquationNode(AccentEquationNode_Impl* impl)](./accentequationnode/) | Constructs from an implementation object. |
| [AccentEquationNode(const AccentEquationNode\& src)](./accentequationnode/) | Copy constructor. |
| [AccentEquationNode(const EquationNode\& src)](./accentequationnode/) | Constructs from a parent object. |
| [AddChild(EquationNodeType equationType)](../equationnode/addchild/) | Insert a node of the specified type at the end of the child node list of the current node. |
| [AddChild(const EquationNode\& node)](../equationnode/addchild/) | Inserts the specified node at the end of the current node's list of child nodes. |
| static [CreateNode(EquationNodeType equationType, const Workbook\& workbook, const EquationNode\& parent)](../equationnode/createnode/) | Create a node of the specified type. |
| [EquationNode(EquationNode_Impl* impl)](../equationnode/equationnode/) | Constructs from an implementation object. |
| [EquationNode(const EquationNode\& src)](../equationnode/equationnode/) | Copy constructor. |
| [EquationNode(const FontSetting\& src)](../equationnode/equationnode/) | Constructs from a parent object. |
| [FontSetting(int32_t startIndex, int32_t length, const WorksheetCollection\& sheets)](../../aspose.cells/fontsetting/fontsetting/) |  |
| [FontSetting(FontSetting_Impl* impl)](../../aspose.cells/fontsetting/fontsetting/) | Constructs from an implementation object. |
| [FontSetting(const FontSetting\& src)](../../aspose.cells/fontsetting/fontsetting/) | Copy constructor. |
| [GetAccentCharacter()](./getaccentcharacter/) | This attribute specifies the type of combining diacritical mark attached to the base of the accent function. The default accent character is U+0302. It is strongly recommended to use attribute AccentType to set accent character. Use this property setting if you cannot find the character you need in a known type. |
| [GetAccentCharacterType()](./getaccentcharactertype/) | Specify combining characters by type value. |
| [GetChild(int32_t index)](../equationnode/getchild/) | Returns the node at the specified index among the children of the current node. |
| [GetEquationType()](../equationnode/getequationtype/) | Get the equation type of the current node. |
| [GetFont()](../../aspose.cells/fontsetting/getfont/) | Returns the font of this object. |
| [GetLength()](../../aspose.cells/fontsetting/getlength/) | Gets the length of the characters. |
| [GetParentNode()](../equationnode/getparentnode/) | Specifies the parent node of the current node. |
| [GetStartIndex()](../../aspose.cells/fontsetting/getstartindex/) | Gets the start index of the characters. |
| [GetTextOptions()](../../aspose.cells/fontsetting/gettextoptions/) | Returns the text options. |
| [GetType()](../equationnode/gettype/) | Represents the type of the node. |
| [InsertAfter(EquationNodeType equationType)](../equationnode/insertafter/) | Inserts the specified node after the current node. |
| [InsertBefore(EquationNodeType equationType)](../equationnode/insertbefore/) | Inserts the specified node before the current node. |
| [InsertChild(int32_t index, EquationNodeType equationType)](../equationnode/insertchild/) | Inserts a node of the specified type at the specified index position in the current node's child node list. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const AccentEquationNode\& src)](./operator_asm/) | operator= |
| [operator=(const EquationNode\& src)](../equationnode/operator_asm/) | operator= |
| [operator=(const FontSetting\& src)](../../aspose.cells/fontsetting/operator_asm/) | operator= |
| [Remove()](../equationnode/remove/) | Removes itself from the parent. |
| [RemoveAllChildren()](../equationnode/removeallchildren/) | Removes all the child nodes of the current node. |
| [RemoveChild(const EquationNode\& node)](../equationnode/removechild/) | Removes the specified node from the current node's children. |
| [RemoveChild(int32_t index)](../equationnode/removechild/) | Removes the node at the specified index from the current node's children. |
| [SetAccentCharacter(const U16String\& value)](./setaccentcharacter/) | This attribute specifies the type of combining diacritical mark attached to the base of the accent function. The default accent character is U+0302. It is strongly recommended to use attribute AccentType to set accent character. Use this property setting if you cannot find the character you need in a known type. |
| [SetAccentCharacter(const char16_t* value)](./setaccentcharacter/) | This attribute specifies the type of combining diacritical mark attached to the base of the accent function. The default accent character is U+0302. It is strongly recommended to use attribute AccentType to set accent character. Use this property setting if you cannot find the character you need in a known type. |
| [SetAccentCharacterType(EquationCombiningCharacterType value)](./setaccentcharactertype/) | Specify combining characters by type value. |
| [SetParentNode(const EquationNode\& value)](../equationnode/setparentnode/) | Specifies the parent node of the current node. |
| [SetWordArtStyle(PresetWordArtStyle style)](../../aspose.cells/fontsetting/setwordartstyle/) | Sets the preset WordArt style. |
| [ToLaTeX()](../equationnode/tolatex/) | Conver this equtation to LaTeX expression. |
| [ToMathML()](../equationnode/tomathml/) | Conver this equtation to MathML expression. |
| [~AccentEquationNode()](./~accentequationnode/) | Destructor. |
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
