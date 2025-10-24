##Aspose::Cells::Slicers::SlicerCacheItemCollection class
'Aspose::Cells::Slicers::SlicerCacheItemCollection class. Represent the collection of SlicerCacheItem in C++.'
## SlicerCacheItemCollection class
Represent the collection of [SlicerCacheItem](../slicercacheitem/).
```cpp
class SlicerCacheItemCollection
```
## Methods
| Method | Description |
| --- | --- |
| [Get(int32_t index)](./get/) | Gets the [SlicerCacheItem](../slicercacheitem/) object by index. |
| [GetCount()](./getcount/) | Gets the count of the [SlicerCacheItem](../slicercacheitem/). |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const SlicerCacheItemCollection\& src)](./operator_asm/) | operator= |
| [SlicerCacheItemCollection(SlicerCacheItemCollection_Impl* impl)](./slicercacheitemcollection/) | Constructs from an implementation object. |
| [SlicerCacheItemCollection(const SlicerCacheItemCollection\& src)](./slicercacheitemcollection/) | Copy constructor. |
| [~SlicerCacheItemCollection()](./~slicercacheitemcollection/) | Destructor. |
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
cells.Get(5, 0).PutValue(u"grape");
cells.Get(6, 0).PutValue(u"blueberry");
cells.Get(7, 0).PutValue(u"kiwi");
cells.Get(8, 0).PutValue(u"cherry");
cells.Get(0, 1).PutValue(u"year");
cells.Get(1, 1).PutValue(2020);
cells.Get(2, 1).PutValue(2020);
cells.Get(3, 1).PutValue(2020);
cells.Get(4, 1).PutValue(2020);
cells.Get(5, 1).PutValue(2021);
cells.Get(6, 1).PutValue(2021);
cells.Get(7, 1).PutValue(2021);
cells.Get(8, 1).PutValue(2021);
cells.Get(0, 2).PutValue(u"amount");
cells.Get(1, 2).PutValue(50);
cells.Get(2, 2).PutValue(60);
cells.Get(3, 2).PutValue(70);
cells.Get(4, 2).PutValue(80);
cells.Get(5, 2).PutValue(90);
cells.Get(6, 2).PutValue(100);
cells.Get(7, 2).PutValue(110);
cells.Get(8, 2).PutValue(120);
PivotTableCollection pivots = sheet.GetPivotTables();
int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots.Get(pivotIndex);
pivot.AddFieldToArea(PivotFieldType::Row, "fruit");
pivot.AddFieldToArea(PivotFieldType::Column, "year");
pivot.AddFieldToArea(PivotFieldType::Data, "amount");
pivot.SetPivotTableStyleType(PivotTableStyleType::PivotTableStyleMedium10);
pivot.RefreshData();
pivot.CalculateData();
SlicerCollection slicers = sheet.GetSlicers();
int slicerIndex = slicers.Add(pivot, "E12", "fruit");
Slicer slicer = slicers.Get(slicerIndex);
slicer.SetStyleType(SlicerStyleType::SlicerStyleLight2);
SlicerCacheItemCollection items = slicer.GetSlicerCache().GetSlicerCacheItems();
book.Save("out.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Slicers](../)
* Library [Aspose.Cells for C++](../../)
