##Aspose::Cells::Row class
'Aspose::Cells::Row class. Represents a single row in a worksheet in C++.'
## Row class
Represents a single row in a worksheet.
```cpp
class Row
```
## Methods
| Method | Description |
| --- | --- |
| [ApplyStyle(const Style\& style, const StyleFlag\& flag)](./applystyle/) | Applies formats for a whole row. |
| [CopySettings(const Row\& source, bool checkStyle)](./copysettings/) | Copy settings of row, such as style, height, visibility, ...etc. |
| [Equals(const Aspose::Cells::Object\& obj)](./equals/) | Checks whether this object refers to the same row with another. |
| [Equals(const Row\& row)](./equals/) | Checks whether this object refers to the same row with another row object. |
| [Get(int32_t column)](./get/) | Gets the cell. |
| [GetCellByIndex(int32_t index)](./getcellbyindex/) | Get the cell by specific index in the cells collection of this row. |
| [GetCellOrNull(int32_t column)](./getcellornull/) | Gets the cell or null in the specific index. |
| [GetEnumerator()](./getenumerator/) | Gets the cells enumerator. |
| [GetEnumerator(bool reversed, bool sync)](./getenumerator/) | Gets an enumerator that iterates cells through this row. |
| [GetFirstCell()](./getfirstcell/) | Gets the first cell object in the row. |
| [GetFirstDataCell()](./getfirstdatacell/) | Gets the first non-blank cell in the row. |
| [GetGroupLevel()](./getgrouplevel/) | Gets the group level of the row. |
| [GetHasCustomStyle()](./gethascustomstyle/) | Indicates whether this row has custom style settings(different from the default one inherited from workbook). |
| [GetHeight()](./getheight/) | Gets and sets the row height in unit of Points. |
| [GetIndex()](./getindex/) | Gets the index of this row. |
| [GetLastCell()](./getlastcell/) | Gets the last cell object in the row. |
| [GetLastDataCell()](./getlastdatacell/) | Gets the last non-blank cell in the row. |
| [GetStyle()](./getstyle/) | Gets the style of this row. |
| [IsBlank()](./isblank/) | Indicates whether the row contains any data. |
| [IsCollapsed()](./iscollapsed/) | whether the row is collapsed |
| [IsHeightMatched()](./isheightmatched/) | Indicates whether the row height matches current default font setting of the workbook. True of this property also denotes the row height is "automatic" without custom height value set by user. |
| [IsHidden()](./ishidden/) | Indicates whether the row is hidden. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Row\& src)](./operator_asm/) | operator= |
| [Row(Row_Impl* impl)](./row/) | Constructs from an implementation object. |
| [Row(const Row\& src)](./row/) | Copy constructor. |
| [SetGroupLevel(uint8_t value)](./setgrouplevel/) | Gets the group level of the row. |
| [SetHeight(double value)](./setheight/) | Gets and sets the row height in unit of Points. |
| [SetIsCollapsed(bool value)](./setiscollapsed/) | whether the row is collapsed |
| [SetIsHeightMatched(bool value)](./setisheightmatched/) | Indicates whether the row height matches current default font setting of the workbook. True of this property also denotes the row height is "automatic" without custom height value set by user. |
| [SetIsHidden(bool value)](./setishidden/) | Indicates whether the row is hidden. |
| [SetStyle(const Style\& style)](./setstyle/) | Sets the style of this row. |
| [~Row()](./~row/) | Destructor. |
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
//Get first row
Row row = worksheet.GetCells().GetRows().Get(0);
//Apply Style to first row
row.ApplyStyle(style, styleFlag);
//Saving the Excel file
workbook.Save(u"book1.xls");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
