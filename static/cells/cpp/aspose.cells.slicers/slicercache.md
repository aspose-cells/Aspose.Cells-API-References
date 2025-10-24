##Aspose::Cells::Slicers::SlicerCache class
'Aspose::Cells::Slicers::SlicerCache class. Represent summary description of slicer cache in C++.'
## SlicerCache class
Represent summary description of slicer cache.
```cpp
class SlicerCache
```
## Methods
| Method | Description |
| --- | --- |
| [GetCrossFilterType()](./getcrossfiltertype/) | Returns or sets whether a slicer is participating in cross filtering with other slicers that share the same slicer cache, and how cross filtering is displayed. Read/write. |
| [GetList()](./getlist/) | Returns whether the slicer associated with the specified slicer cache is based on an Non-OLAP data source. Read-only. |
| [GetName()](./getname/) | Returns the name of the slicer cache. |
| [GetSlicerCacheItems()](./getslicercacheitems/) | Returns a [SlicerCacheItem](../slicercacheitem/) collection that contains the collection of all items in the slicer cache. Read-only. |
| [GetSourceName()](./getsourcename/) | Returns the name of this slicer cache. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const SlicerCache\& src)](./operator_asm/) | operator= |
| [SetCrossFilterType(SlicerCacheCrossFilterType value)](./setcrossfiltertype/) | Returns or sets whether a slicer is participating in cross filtering with other slicers that share the same slicer cache, and how cross filtering is displayed. Read/write. |
| [SlicerCache(SlicerCache_Impl* impl)](./slicercache/) | Constructs from an implementation object. |
| [SlicerCache(const SlicerCache\& src)](./slicercache/) | Copy constructor. |
| [~SlicerCache()](./~slicercache/) | Destructor. |
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
int pivotIndex = pivots.Add(u"=Sheet1!A1:C9", u"A12", u"TestPivotTable");
PivotTable pivot = pivots.Get(pivotIndex);
pivot.AddFieldToArea(PivotFieldType::Row, u"fruit");
pivot.AddFieldToArea(PivotFieldType::Column, u"year");
pivot.AddFieldToArea(PivotFieldType::Data, u"amount");
pivot.SetPivotTableStyleType(PivotTableStyleType::PivotTableStyleMedium10);
pivot.RefreshData();
pivot.CalculateData();
SlicerCollection slicers = sheet.GetSlicers();
int slicerIndex = slicers.Add(pivot, "E12", "fruit");
Slicer slicer = slicers.Get(slicerIndex);
slicer.SetStyleType(SlicerStyleType::SlicerStyleLight2);
//Get SlicerCache object of current slicer
SlicerCache slicerCache = slicer.GetSlicerCache();
book.Save("out.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Slicers](../)
* Library [Aspose.Cells for C++](../../)
