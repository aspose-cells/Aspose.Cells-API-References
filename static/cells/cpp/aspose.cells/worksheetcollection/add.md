##Aspose::Cells::WorksheetCollection::Add method
'Aspose::Cells::WorksheetCollection::Add method. Adds a worksheet to the collection in C++.'
## WorksheetCollection::Add(SheetType) method
Adds a worksheet to the collection.
```cpp
int32_t Aspose::Cells::WorksheetCollection::Add(SheetType type)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | SheetType | [Worksheet](../../worksheet/) type. |
## ReturnValue
[Worksheet](../../worksheet/) object index.
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
workbook.GetWorksheets().Add(SheetType::Chart);
Cells cells = workbook.GetWorksheets().Get(0).GetCells();
cells.Get(u"c2").PutValue(5000);
cells.Get(u"c3").PutValue(3000);
cells.Get(u"c4").PutValue(4000);
cells.Get(u"c5").PutValue(5000);
cells.Get(u"c6").PutValue(6000);
ChartCollection charts = workbook.GetWorksheets().Get(1).GetCharts();
int chartIndex = charts.Add(ChartType::Column, 10, 10, 20, 20);
Chart chart = charts.Get(chartIndex);
chart.GetNSeries().Add(u"Sheet1!C2:C6", true);
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Enum [SheetType](../../sheettype/)
* Class [WorksheetCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## WorksheetCollection::Add() method
Adds a worksheet to the collection.
```cpp
int32_t Aspose::Cells::WorksheetCollection::Add()
```
## ReturnValue
[Worksheet](../../worksheet/) object index.
## See Also
* Class [Vector](../../vector/)
* Class [WorksheetCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## WorksheetCollection::Add(const U16String\&) method
Adds a worksheet to the collection.
```cpp
Worksheet Aspose::Cells::WorksheetCollection::Add(const U16String &sheetName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | const U16String\& | [Worksheet](../../worksheet/) name |
## ReturnValue
[Worksheet](../../worksheet/) object.
## See Also
* Class [Worksheet](../../worksheet/)
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [WorksheetCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## WorksheetCollection::Add(const char16_t*) method
Adds a worksheet to the collection.
```cpp
Worksheet Aspose::Cells::WorksheetCollection::Add(const char16_t *sheetName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | const char16_t* | [Worksheet](../../worksheet/) name |
## ReturnValue
[Worksheet](../../worksheet/) object.
## See Also
* Class [Worksheet](../../worksheet/)
* Class [Vector](../../vector/)
* Class [WorksheetCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
