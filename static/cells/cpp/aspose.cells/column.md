##Aspose::Cells::Column class
'Aspose::Cells::Column class. Represents a single column in a worksheet in C++.'
## Column class
Represents a single column in a worksheet.
```cpp
class Column
```
## Methods
| Method | Description |
| --- | --- |
| [ApplyStyle(const Style\& style, const StyleFlag\& flag)](./applystyle/) | Applies formats for a whole column. |
| [Column(Column_Impl* impl)](./column/) | Constructs from an implementation object. |
| [Column(const Column\& src)](./column/) | Copy constructor. |
| [GetGroupLevel()](./getgrouplevel/) | Gets the group level of the column. |
| [GetHasCustomStyle()](./gethascustomstyle/) | Indicates whether this column has custom style settings(different from the default one inherited from workbook). |
| [GetIndex()](./getindex/) | Gets the index of this column. |
| [GetStyle()](./getstyle/) | Gets the style of this column. |
| [GetWidth()](./getwidth/) | Gets and sets the column width in unit of characters. |
| [IsCollapsed()](./iscollapsed/) | whether the column is collapsed |
| [IsHidden()](./ishidden/) | Indicates whether the column is hidden. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Column\& src)](./operator_asm/) | operator= |
| [SetGroupLevel(uint8_t value)](./setgrouplevel/) | Gets the group level of the column. |
| [SetIsCollapsed(bool value)](./setiscollapsed/) | whether the column is collapsed |
| [SetIsHidden(bool value)](./setishidden/) | Indicates whether the column is hidden. |
| [SetStyle(const Style\& style)](./setstyle/) | Sets the style of this column. |
| [SetWidth(double value)](./setwidth/) | Gets and sets the column width in unit of characters. |
| [~Column()](./~column/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
//Obtaining the reference of the first worksheet
Worksheet worksheet = workbook.GetWorksheets().Get(0);
Style style = workbook.CreateStyle();
//Setting the background color to Blue
style.SetBackgroundColor(Color{ 0xff, 0, 0, 0xff });
//Setting the foreground color to Red
style.SetForegroundColor(Color{ 0xff, 0xff, 0, 0 });
//setting Background Pattern
style.SetPattern(BackgroundType::DiagonalStripe);
//New Style Flag
StyleFlag styleFlag;
//Set All Styles
styleFlag.SetAll(true);
//Get first Column
Column column = worksheet.GetCells().GetColumns().Get(0);
//Apply Style to first Column
column.ApplyStyle(style, styleFlag);
//Saving the Excel file
workbook.Save(u"book1.xls");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
