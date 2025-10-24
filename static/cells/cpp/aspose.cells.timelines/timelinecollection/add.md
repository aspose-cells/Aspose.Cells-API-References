##Aspose::Cells::Timelines::TimelineCollection::Add method
'Aspose::Cells::Timelines::TimelineCollection::Add method. Add a new Timeline using PivotTable as data source in C++.'
## TimelineCollection::Add(const PivotTable\&, int32_t, int32_t, const U16String\&) method
Add a new [Timeline](../../timeline/) using PivotTable as data source.
```cpp
int32_t Aspose::Cells::Timelines::TimelineCollection::Add(const PivotTable &pivot, int32_t row, int32_t column, const U16String &baseFieldName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | const PivotTable\& | PivotTable object |
| row | int32_t | [Row](../../../aspose.cells/row/) index of the cell in the upper-left corner of the [Timeline](../../timeline/) range. |
| column | int32_t | [Column](../../../aspose.cells/column/) index of the cell in the upper-left corner of the [Timeline](../../timeline/) range. |
| baseFieldName | const U16String\& | The name of PivotField in PivotTable.BaseFields |
## ReturnValue
The new add [Timeline](../../timeline/) index
## Examples
```cpp
//Add a new Timeline using PivotTable as data source
U16String val = u"date";
sheet.GetTimelines().Add(pivotTable, 10, 5, val);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [TimelineCollection](../)
* Namespace [Aspose::Cells::Timelines](../../)
* Library [Aspose.Cells for C++](../../../)
## TimelineCollection::Add(const PivotTable\&, int32_t, int32_t, const char16_t*) method
Add a new [Timeline](../../timeline/) using PivotTable as data source.
```cpp
int32_t Aspose::Cells::Timelines::TimelineCollection::Add(const PivotTable &pivot, int32_t row, int32_t column, const char16_t *baseFieldName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | const PivotTable\& | PivotTable object |
| row | int32_t | [Row](../../../aspose.cells/row/) index of the cell in the upper-left corner of the [Timeline](../../timeline/) range. |
| column | int32_t | [Column](../../../aspose.cells/column/) index of the cell in the upper-left corner of the [Timeline](../../timeline/) range. |
| baseFieldName | const char16_t* | The name of PivotField in PivotTable.BaseFields |
## ReturnValue
The new add [Timeline](../../timeline/) index
## Examples
```cpp
//Add a new Timeline using PivotTable as data source
sheet.GetTimelines().Add(pivotTable, 10, 5, u"date");
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* Class [TimelineCollection](../)
* Namespace [Aspose::Cells::Timelines](../../)
* Library [Aspose.Cells for C++](../../../)
## TimelineCollection::Add(const PivotTable\&, const U16String\&, const U16String\&) method
Add a new [Timeline](../../timeline/) using PivotTable as data source.
```cpp
int32_t Aspose::Cells::Timelines::TimelineCollection::Add(const PivotTable &pivot, const U16String &destCellName, const U16String &baseFieldName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | const PivotTable\& | PivotTable object |
| destCellName | const U16String\& | The cell name in the upper-left corner of the [Timeline](../../timeline/) range. |
| baseFieldName | const U16String\& | The name of PivotField in PivotTable.BaseFields |
## ReturnValue
The new add [Timeline](../../timeline/) index
## Examples
```cpp
//Add a new Timeline using PivotTable as data source
U16String val1 = u"i15";
U16String val2 = u"date";
sheet.GetTimelines().Add(pivotTable, val1, val2);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [TimelineCollection](../)
* Namespace [Aspose::Cells::Timelines](../../)
* Library [Aspose.Cells for C++](../../../)
## TimelineCollection::Add(const PivotTable\&, const char16_t*, const char16_t*) method
Add a new [Timeline](../../timeline/) using PivotTable as data source.
```cpp
int32_t Aspose::Cells::Timelines::TimelineCollection::Add(const PivotTable &pivot, const char16_t *destCellName, const char16_t *baseFieldName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | const PivotTable\& | PivotTable object |
| destCellName | const char16_t* | The cell name in the upper-left corner of the [Timeline](../../timeline/) range. |
| baseFieldName | const char16_t* | The name of PivotField in PivotTable.BaseFields |
## ReturnValue
The new add [Timeline](../../timeline/) index
## Examples
```cpp
//Add a new Timeline using PivotTable as data source
sheet.GetTimelines().Add(pivotTable, u"i15", u"date");
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* Class [TimelineCollection](../)
* Namespace [Aspose::Cells::Timelines](../../)
* Library [Aspose.Cells for C++](../../../)
## TimelineCollection::Add(const PivotTable\&, int32_t, int32_t, int32_t) method
Add a new [Timeline](../../timeline/) using PivotTable as data source.
```cpp
int32_t Aspose::Cells::Timelines::TimelineCollection::Add(const PivotTable &pivot, int32_t row, int32_t column, int32_t baseFieldIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | const PivotTable\& | PivotTable object |
| row | int32_t | [Row](../../../aspose.cells/row/) index of the cell in the upper-left corner of the [Timeline](../../timeline/) range. |
| column | int32_t | [Column](../../../aspose.cells/column/) index of the cell in the upper-left corner of the [Timeline](../../timeline/) range. |
| baseFieldIndex | int32_t | The index of PivotField in PivotTable.BaseFields |
## ReturnValue
The new add [Timeline](../../timeline/) index
## Examples
```cpp
//Add a new Timeline using PivotTable as data source
sheet.GetTimelines().Add(pivotTable, 15, 5, 1);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* Class [TimelineCollection](../)
* Namespace [Aspose::Cells::Timelines](../../)
* Library [Aspose.Cells for C++](../../../)
## TimelineCollection::Add(const PivotTable\&, const U16String\&, int32_t) method
Add a new [Timeline](../../timeline/) using PivotTable as data source.
```cpp
int32_t Aspose::Cells::Timelines::TimelineCollection::Add(const PivotTable &pivot, const U16String &destCellName, int32_t baseFieldIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | const PivotTable\& | PivotTable object |
| destCellName | const U16String\& | The cell name in the upper-left corner of the [Timeline](../../timeline/) range. |
| baseFieldIndex | int32_t | The index of PivotField in PivotTable.BaseFields |
## ReturnValue
The new add [Timeline](../../timeline/) index
## Examples
```cpp
//Add a new Timeline using PivotTable as data source
U16String val = u"i5";
sheet.GetTimelines().Add(pivotTable, val, 1);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [TimelineCollection](../)
* Namespace [Aspose::Cells::Timelines](../../)
* Library [Aspose.Cells for C++](../../../)
## TimelineCollection::Add(const PivotTable\&, const char16_t*, int32_t) method
Add a new [Timeline](../../timeline/) using PivotTable as data source.
```cpp
int32_t Aspose::Cells::Timelines::TimelineCollection::Add(const PivotTable &pivot, const char16_t *destCellName, int32_t baseFieldIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | const PivotTable\& | PivotTable object |
| destCellName | const char16_t* | The cell name in the upper-left corner of the [Timeline](../../timeline/) range. |
| baseFieldIndex | int32_t | The index of PivotField in PivotTable.BaseFields |
## ReturnValue
The new add [Timeline](../../timeline/) index
## Examples
```cpp
//Add a new Timeline using PivotTable as data source
sheet.GetTimelines().Add(pivotTable, u"i5", 1);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* Class [TimelineCollection](../)
* Namespace [Aspose::Cells::Timelines](../../)
* Library [Aspose.Cells for C++](../../../)
## TimelineCollection::Add(const PivotTable\&, int32_t, int32_t, const PivotField\&) method
Add a new [Timeline](../../timeline/) using PivotTable as data source.
```cpp
int32_t Aspose::Cells::Timelines::TimelineCollection::Add(const PivotTable &pivot, int32_t row, int32_t column, const PivotField &baseField)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | const PivotTable\& | PivotTable object |
| row | int32_t | [Row](../../../aspose.cells/row/) index of the cell in the upper-left corner of the [Timeline](../../timeline/) range. |
| column | int32_t | [Column](../../../aspose.cells/column/) index of the cell in the upper-left corner of the [Timeline](../../timeline/) range. |
| baseField | const PivotField\& | The PivotField in PivotTable.BaseFields |
## ReturnValue
The new add [Timeline](../../timeline/) index
## Examples
```cpp
//Add a new Timeline using PivotTable as data source
sheet.GetTimelines().Add(pivotTable, 20, 5, pivotTable.GetBaseFields().Get(1));
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* Class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* Class [TimelineCollection](../)
* Namespace [Aspose::Cells::Timelines](../../)
* Library [Aspose.Cells for C++](../../../)
## TimelineCollection::Add(const PivotTable\&, const U16String\&, const PivotField\&) method
Add a new [Timeline](../../timeline/) using PivotTable as data source.
```cpp
int32_t Aspose::Cells::Timelines::TimelineCollection::Add(const PivotTable &pivot, const U16String &destCellName, const PivotField &baseField)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | const PivotTable\& | PivotTable object |
| destCellName | const U16String\& | The cell name in the upper-left corner of the [Timeline](../../timeline/) range. |
| baseField | const PivotField\& | The PivotField in PivotTable.BaseFields |
## ReturnValue
The new add [Timeline](../../timeline/) index
## Examples
```cpp
//Add a new Timeline using PivotTable as data source
U16String val = u"i10";
sheet.GetTimelines().Add(pivotTable, val, pivotTable.GetBaseFields().Get(1));
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* Class [TimelineCollection](../)
* Namespace [Aspose::Cells::Timelines](../../)
* Library [Aspose.Cells for C++](../../../)
## TimelineCollection::Add(const PivotTable\&, const char16_t*, const PivotField\&) method
Add a new [Timeline](../../timeline/) using PivotTable as data source.
```cpp
int32_t Aspose::Cells::Timelines::TimelineCollection::Add(const PivotTable &pivot, const char16_t *destCellName, const PivotField &baseField)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | const PivotTable\& | PivotTable object |
| destCellName | const char16_t* | The cell name in the upper-left corner of the [Timeline](../../timeline/) range. |
| baseField | const PivotField\& | The PivotField in PivotTable.BaseFields |
## ReturnValue
The new add [Timeline](../../timeline/) index
## Examples
```cpp
//Add a new Timeline using PivotTable as data source
sheet.GetTimelines().Add(pivotTable, u"i10", pivotTable.GetBaseFields().Get(1));
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* Class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* Class [TimelineCollection](../)
* Namespace [Aspose::Cells::Timelines](../../)
* Library [Aspose.Cells for C++](../../../)
