##Aspose::Cells::ColumnCollection class
'Aspose::Cells::ColumnCollection class. Collection of the Column objects that represent the individual column(setting)s in a worksheet. The Column object only represents the settings such as column width, styles, .etc. for the whole column, has nothing to do with the fact that there are non-empty cells(data) or not in corresponding column. And the "Count" of this collection only represents the count Column objects that have been instantiated in this collection, has nothing to do with the fact that there are non-empty cells(data) or not in the worksheet in C++.'
## ColumnCollection class
Collection of the [Column](../column/) objects that represent the individual column(setting)s in a worksheet. The [Column](../column/) object only represents the settings such as column width, styles, .etc. for the whole column, has nothing to do with the fact that there are non-empty cells(data) or not in corresponding column. And the "Count" of this collection only represents the count [Column](../column/) objects that have been instantiated in this collection, has nothing to do with the fact that there are non-empty cells(data) or not in the worksheet.
```cpp
class ColumnCollection
```
## Methods
| Method | Description |
| --- | --- |
| [ColumnCollection(ColumnCollection_Impl* impl)](./columncollection/) | Constructs from an implementation object. |
| [ColumnCollection(const ColumnCollection\& src)](./columncollection/) | Copy constructor. |
| [Get(int32_t columnIndex)](./get/) | Gets a [Column](../column/) object by column index. The [Column](../column/) object of given column index will be instantiated if it does not exist before. |
| [GetColumnByIndex(int32_t index)](./getcolumnbyindex/) | Gets the [Column](../column/) object by the position in the list. |
| [GetCount()](./getcount/) |  |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ColumnCollection\& src)](./operator_asm/) | operator= |
| [~ColumnCollection()](./~columncollection/) | Destructor. |
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
//Add new Style to Workbook
Style style = workbook.CreateStyle();
//Setting the background color to Blue
style.SetForegroundColor(Color{ 0xff, 0, 0, 0xff });
//setting Background Pattern
style.SetPattern(BackgroundType::Solid);
//New Style Flag
StyleFlag styleFlag;
//Set All Styles
styleFlag.SetAll(true);
//Change the default width of first ten columns
for (int i = 0; i < 10; i++)
{
worksheet.GetCells().GetColumns().Get(i).SetWidth(20);
}
//Get the Column with non default formatting
ColumnCollection columns = worksheet.GetCells().GetColumns();
for (int i = 0; i < columns.GetCount(); ++i)
{
Column column = columns.Get(i);
//Apply Style to first ten Columns
column.ApplyStyle(style, styleFlag);
}
//Saving the Excel file
workbook.Save(u"book1.xls");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
