##Aspose::Cells::Drawing::Equations::MatrixEquationNode class
'Aspose::Cells::Drawing::Equations::MatrixEquationNode class. This class specifies the Matrix equation, consisting of one or more elements laid out in one or more rows and one or more columns in C++.'
## MatrixEquationNode class
This class specifies the Matrix equation, consisting of one or more elements laid out in one or more rows and one or more columns.
```cpp
class MatrixEquationNode : public Aspose::Cells::Drawing::Equations::EquationNode
```
## Methods
| Method | Description |
| --- | --- |
| [AddChild(EquationNodeType equationType)](../equationnode/addchild/) | Insert a node of the specified type at the end of the child node list of the current node. |
| [AddChild(const EquationNode\& node)](../equationnode/addchild/) | Inserts the specified node at the end of the current node's list of child nodes. |
| static [CreateNode(EquationNodeType equationType, const Workbook\& workbook, const EquationNode\& parent)](../equationnode/createnode/) | Create a node of the specified type. |
| [Equals(const Aspose::Cells::Object\& obj)](./equals/) | Determine whether the current equation node is equal to the specified node. |
| [EquationNode(EquationNode_Impl* impl)](../equationnode/equationnode/) | Constructs from an implementation object. |
| [EquationNode(const EquationNode\& src)](../equationnode/equationnode/) | Copy constructor. |
| [EquationNode(const FontSetting\& src)](../equationnode/equationnode/) | Constructs from a parent object. |
| [FontSetting(int32_t startIndex, int32_t length, const WorksheetCollection\& sheets)](../../aspose.cells/fontsetting/fontsetting/) |  |
| [FontSetting(FontSetting_Impl* impl)](../../aspose.cells/fontsetting/fontsetting/) | Constructs from an implementation object. |
| [FontSetting(const FontSetting\& src)](../../aspose.cells/fontsetting/fontsetting/) | Copy constructor. |
| [GetBaseJc()](./getbasejc/) | This attribute specifies the justification of the matrix. Text outside of the matrix can be aligned with the bottom, top, or center of a matrix function. Default, the matrix assumes center justification. |
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
| [IsHidePlaceholder()](./ishideplaceholder/) | This attribute specifies the Hide Placeholders property on a matrix. When this property is on, placeholders do not appear in the matrix.Default, placeholders do appear such that the locations where text can be inserted are made visible. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [MatrixEquationNode(MatrixEquationNode_Impl* impl)](./matrixequationnode/) | Constructs from an implementation object. |
| [MatrixEquationNode(const MatrixEquationNode\& src)](./matrixequationnode/) | Copy constructor. |
| [MatrixEquationNode(const EquationNode\& src)](./matrixequationnode/) | Constructs from a parent object. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const MatrixEquationNode\& src)](./operator_asm/) | operator= |
| [operator=(const EquationNode\& src)](../equationnode/operator_asm/) | operator= |
| [operator=(const FontSetting\& src)](../../aspose.cells/fontsetting/operator_asm/) | operator= |
| [Remove()](../equationnode/remove/) | Removes itself from the parent. |
| [RemoveAllChildren()](../equationnode/removeallchildren/) | Removes all the child nodes of the current node. |
| [RemoveChild(const EquationNode\& node)](../equationnode/removechild/) | Removes the specified node from the current node's children. |
| [RemoveChild(int32_t index)](../equationnode/removechild/) | Removes the node at the specified index from the current node's children. |
| [SetBaseJc(EquationVerticalJustificationType value)](./setbasejc/) | This attribute specifies the justification of the matrix. Text outside of the matrix can be aligned with the bottom, top, or center of a matrix function. Default, the matrix assumes center justification. |
| [SetIsHidePlaceholder(bool value)](./setishideplaceholder/) | This attribute specifies the Hide Placeholders property on a matrix. When this property is on, placeholders do not appear in the matrix.Default, placeholders do appear such that the locations where text can be inserted are made visible. |
| [SetParentNode(const EquationNode\& value)](../equationnode/setparentnode/) | Specifies the parent node of the current node. |
| [SetWordArtStyle(PresetWordArtStyle style)](../../aspose.cells/fontsetting/setwordartstyle/) | Sets the preset WordArt style. |
| [ToLaTeX()](../equationnode/tolatex/) | Convert this equtation to LaTeX expression. |
| [ToMathML()](../equationnode/tomathml/) | Convert this equtation to MathML expression. |
| [~EquationNode()](../equationnode/~equationnode/) | Destructor. |
| [~FontSetting()](../../aspose.cells/fontsetting/~fontsetting/) | Destructor. |
| [~MatrixEquationNode()](./~matrixequationnode/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Class [EquationNode](../equationnode/)
* Namespace [Aspose::Cells::Drawing::Equations](../)
* Library [Aspose.Cells for C++](../../)
