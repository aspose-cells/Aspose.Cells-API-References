---
title: Aspose::Cells::Drawing::Equations::EquationNode class
linktitle: EquationNode
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Equations::EquationNode class. Abstract class for deriving other equation nodes in C++.'
type: docs
weight: 800
url: /cpp/aspose.cells.drawing.equations/equationnode/
---
## EquationNode class


Abstract class for deriving other equation nodes.

```cpp
class EquationNode : public Aspose::Cells::FontSetting
```

## Methods

| Method | Description |
| --- | --- |
| [AddChild(EquationNodeType equationType)](./addchild/) | Insert a node of the specified type at the end of the child node list of the current node. |
| [AddChild(const EquationNode\& node)](./addchild/) | Inserts the specified node at the end of the current node's list of child nodes. |
| static [CreateNode(EquationNodeType equationType, const Workbook\& workbook, const EquationNode\& parent)](./createnode/) | Create a node of the specified type. |
| [Equals(const Aspose::Cells::Object\& obj)](./equals/) | Determine whether the current equation node is equal to the specified node. |
| [EquationNode(EquationNode_Impl* impl)](./equationnode/) | Constructs from an implementation object. |
| [EquationNode(const EquationNode\& src)](./equationnode/) | Copy constructor. |
| [EquationNode(const FontSetting\& src)](./equationnode/) | Constructs from a parent object. |
| [FontSetting(int32_t startIndex, int32_t length, const WorksheetCollection\& sheets)](../../aspose.cells/fontsetting/fontsetting/) |  |
| [FontSetting(FontSetting_Impl* impl)](../../aspose.cells/fontsetting/fontsetting/) | Constructs from an implementation object. |
| [FontSetting(const FontSetting\& src)](../../aspose.cells/fontsetting/fontsetting/) | Copy constructor. |
| [GetChild(int32_t index)](./getchild/) | Returns the node at the specified index among the children of the current node. |
| [GetEquationType()](./getequationtype/) | Get the equation type of the current node. |
| [GetFont()](../../aspose.cells/fontsetting/getfont/) | Returns the font of this object. |
| [GetLength()](../../aspose.cells/fontsetting/getlength/) | Gets the length of the characters. |
| [GetParentNode()](./getparentnode/) | Specifies the parent node of the current node. |
| [GetStartIndex()](../../aspose.cells/fontsetting/getstartindex/) | Gets the start index of the characters. |
| [GetTextOptions()](../../aspose.cells/fontsetting/gettextoptions/) | Returns the text options. |
| [GetType()](./gettype/) | Represents the type of the node. |
| [InsertAfter(EquationNodeType equationType)](./insertafter/) | Inserts the specified node after the current node. |
| [InsertBefore(EquationNodeType equationType)](./insertbefore/) | Inserts the specified node before the current node. |
| [InsertChild(int32_t index, EquationNodeType equationType)](./insertchild/) | Inserts a node of the specified type at the specified index position in the current node's child node list. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const EquationNode\& src)](./operator_asm/) | operator= |
| [operator=(const FontSetting\& src)](../../aspose.cells/fontsetting/operator_asm/) | operator= |
| [Remove()](./remove/) | Removes itself from the parent. |
| [RemoveAllChildren()](./removeallchildren/) | Removes all the child nodes of the current node. |
| [RemoveChild(const EquationNode\& node)](./removechild/) | Removes the specified node from the current node's children. |
| [RemoveChild(int32_t index)](./removechild/) | Removes the node at the specified index from the current node's children. |
| [SetParentNode(const EquationNode\& value)](./setparentnode/) | Specifies the parent node of the current node. |
| [SetWordArtStyle(PresetWordArtStyle style)](../../aspose.cells/fontsetting/setwordartstyle/) | Sets the preset WordArt style. |
| [ToLaTeX()](./tolatex/) | Convert this equtation to LaTeX expression. |
| [ToMathML()](./tomathml/) | Convert this equtation to MathML expression. |
| [~EquationNode()](./~equationnode/) | Destructor. |
| [~FontSetting()](../../aspose.cells/fontsetting/~fontsetting/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
// Instantiate a Workbook object that represents Excel file.
Workbook workbook;

// Adds an equation object to the worksheet.
TextBox textBox = workbook.GetWorksheets().Get(0).GetShapes().AddEquation(1, 0, 1, 0, 100, 300);

// Gets the starting node of the equation object
EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

// Inserts a fractional equation.
FractionEquationNode node = (FractionEquationNode)mathNode.AddChild(EquationNodeType::Fraction);
node.SetFractionType(EquationFractionType::Skewed);

U16String str1 = u"A";
EquationComponentNode numerator = (EquationComponentNode)node.AddChild(EquationNodeType::Numerator);
TextRunEquationNode TR = (TextRunEquationNode)(numerator.AddChild(EquationNodeType::Text));
TR.SetText(str1);

U16String str2 = u"B";
EquationComponentNode denominator = (EquationComponentNode)node.AddChild(EquationNodeType::Denominator);
TR = (TextRunEquationNode)(denominator.AddChild(EquationNodeType::Text));
TR.SetText(str2);


//Save the excel file.
workbook.Save(u"exmaple.xlsx");

Aspose::Cells::Cleanup();
```

## See Also

* Class [FontSetting](../../aspose.cells/fontsetting/)
* Namespace [Aspose::Cells::Drawing::Equations](../)
* Library [Aspose.Cells for C++](../../)
