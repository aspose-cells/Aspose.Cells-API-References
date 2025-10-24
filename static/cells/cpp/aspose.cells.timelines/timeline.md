##Aspose::Cells::Timelines::Timeline class
'Aspose::Cells::Timelines::Timeline class. Summary description of Timeline View Due to MS Excel, Excel 2003 does not support Timeline in C++.'
## Timeline class
Summary description of [Timeline](./) View Due to MS Excel, Excel 2003 does not support [Timeline](./).
```cpp
class Timeline
```
## Methods
| Method | Description |
| --- | --- |
| [GetCaption()](./getcaption/) | Returns or sets the caption of the specified [Timeline](./). |
| [GetHeightPixel()](./getheightpixel/) |  **(Deprecated)** Returns or sets the height of the specified timeline, in pixels. |
| [GetLeftPixel()](./getleftpixel/) |  **(Deprecated)** Returns or sets the horizontal offset of timeline shape from its left column, in pixels. |
| [GetName()](./getname/) | Returns or sets the name of the specified [Timeline](./). |
| [GetShape()](./getshape/) | Returns the TimelineShape object associated with this [Timeline](./). Read-only. |
| [GetTopPixel()](./gettoppixel/) |  **(Deprecated)** Returns or sets the vertical offset of timeline shape from its top row, in pixels. |
| [GetWidthPixel()](./getwidthpixel/) |  **(Deprecated)** Returns or sets the width of the specified timeline, in pixels. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Timeline\& src)](./operator_asm/) | operator= |
| [SetCaption(const U16String\& value)](./setcaption/) | Returns or sets the caption of the specified [Timeline](./). |
| [SetCaption(const char16_t* value)](./setcaption/) | Returns or sets the caption of the specified [Timeline](./). |
| [SetHeightPixel(int32_t value)](./setheightpixel/) |  **(Deprecated)** Returns or sets the height of the specified timeline, in pixels. |
| [SetLeftPixel(int32_t value)](./setleftpixel/) |  **(Deprecated)** Returns or sets the horizontal offset of timeline shape from its left column, in pixels. |
| [SetName(const U16String\& value)](./setname/) | Returns or sets the name of the specified [Timeline](./). |
| [SetName(const char16_t* value)](./setname/) | Returns or sets the name of the specified [Timeline](./). |
| [SetTopPixel(int32_t value)](./settoppixel/) |  **(Deprecated)** Returns or sets the vertical offset of timeline shape from its top row, in pixels. |
| [SetWidthPixel(int32_t value)](./setwidthpixel/) |  **(Deprecated)** Returns or sets the width of the specified timeline, in pixels. |
| [Timeline(Timeline_Impl* impl)](./timeline/) | Constructs from an implementation object. |
| [Timeline(const Timeline\& src)](./timeline/) | Copy constructor. |
| [~Timeline()](./~timeline/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook book;
Worksheet sheet = book.GetWorksheets().Get(0);
Cells cells = sheet.GetCells();
cells.Get(0, 0).PutValue(u"fruit");
cells.Get(1, 0).PutValue(u"grape");
cells.Get(2, 0).PutValue(u"blueberry");
cells.Get(3, 0).PutValue(u"kiwi");
cells.Get(4, 0).PutValue(u"cherry");
//Create date style
Style dateStyle = CellsFactory().CreateStyle();
dateStyle.SetCustom(u"m/d/yyyy");
cells.Get(0, 1).PutValue(u"date");
cells.Get(1, 1).PutValue(Date{ 2021, 2, 5 });
cells.Get(2, 1).PutValue(Date{ 2022, 3, 8 });
cells.Get(3, 1).PutValue(Date{ 2023, 4, 10 });
cells.Get(4, 1).PutValue(Date{ 2024, 5, 16 });
//Set date style
cells.Get(1, 1).SetStyle(dateStyle);
cells.Get(2, 1).SetStyle(dateStyle);
cells.Get(3, 1).SetStyle(dateStyle);
cells.Get(4, 1).SetStyle(dateStyle);
cells.Get(0, 2).PutValue(u"amount");
cells.Get(1, 2).PutValue(50);
cells.Get(2, 2).PutValue(60);
cells.Get(3, 2).PutValue(70);
cells.Get(4, 2).PutValue(80);
PivotTableCollection pivots = sheet.GetPivotTables();
//Add a PivotTable
int pivotIndex = pivots.Add(u"=Sheet1!A1:C5", u"A12", u"TestPivotTable");
PivotTable pivot = pivots.Get(pivotIndex);
pivot.AddFieldToArea(PivotFieldType::Row, u"fruit");
pivot.AddFieldToArea(PivotFieldType::Column, u"date");
pivot.AddFieldToArea(PivotFieldType::Data, u"amount");
pivot.SetPivotTableStyleType(PivotTableStyleType::PivotTableStyleMedium10);
//Refresh PivotTable data
pivot.RefreshData();
pivot.CalculateData();
//Add a new Timeline using PivotTable as data source
sheet.GetTimelines().Add(pivot, 10, 5, u"date");
//Get Timeline object
Timeline timelineObj = sheet.GetTimelines().Get(0);
book.Save(u"out.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Timelines](../)
* Library [Aspose.Cells for C++](../../)
