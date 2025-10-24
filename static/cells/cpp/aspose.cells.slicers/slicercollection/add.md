##Aspose::Cells::Slicers::SlicerCollection::Add method
'Aspose::Cells::Slicers::SlicerCollection::Add method. Add a new Slicer using PivotTable as data source in C++.'
## SlicerCollection::Add(const PivotTable\&, const U16String\&, const U16String\&) method
Add a new [Slicer](../../slicer/) using PivotTable as data source.
```cpp
int32_t Aspose::Cells::Slicers::SlicerCollection::Add(const PivotTable &pivot, const U16String &destCellName, const U16String &baseFieldName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | const PivotTable\& | PivotTable object |
| destCellName | const U16String\& | The cell in the upper-left corner of the [Slicer](../../slicer/) range. |
| baseFieldName | const U16String\& | The name of PivotField in PivotTable.BaseFields |
## ReturnValue
The new add [Slicer](../../slicer/) index
## Examples
```cpp
U16String val1 = u"E3";
U16String val2 = u"fruit";
slicers.Add(pivotTable, val1, val2);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [SlicerCollection](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
## SlicerCollection::Add(const PivotTable\&, const char16_t*, const char16_t*) method
Add a new [Slicer](../../slicer/) using PivotTable as data source.
```cpp
int32_t Aspose::Cells::Slicers::SlicerCollection::Add(const PivotTable &pivot, const char16_t *destCellName, const char16_t *baseFieldName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | const PivotTable\& | PivotTable object |
| destCellName | const char16_t* | The cell in the upper-left corner of the [Slicer](../../slicer/) range. |
| baseFieldName | const char16_t* | The name of PivotField in PivotTable.BaseFields |
## ReturnValue
The new add [Slicer](../../slicer/) index
## Examples
```cpp
slicers.Add(pivot, u"E3", u"fruit");
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* Class [SlicerCollection](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
## SlicerCollection::Add(const PivotTable\&, int32_t, int32_t, const U16String\&) method
Add a new [Slicer](../../slicer/) using PivotTable as data source.
```cpp
int32_t Aspose::Cells::Slicers::SlicerCollection::Add(const PivotTable &pivot, int32_t row, int32_t column, const U16String &baseFieldName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | const PivotTable\& | PivotTable object |
| row | int32_t | [Row](../../../aspose.cells/row/) index of the cell in the upper-left corner of the [Slicer](../../slicer/) range. |
| column | int32_t | [Column](../../../aspose.cells/column/) index of the cell in the upper-left corner of the [Slicer](../../slicer/) range. |
| baseFieldName | const U16String\& | The name of PivotField in PivotTable.BaseFields |
## ReturnValue
The new add [Slicer](../../slicer/) index
## Examples
```cpp
U16String val = u"fruit";
slicers.Add(pivotTable, 20, 12, val);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [SlicerCollection](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
## SlicerCollection::Add(const PivotTable\&, int32_t, int32_t, const char16_t*) method
Add a new [Slicer](../../slicer/) using PivotTable as data source.
```cpp
int32_t Aspose::Cells::Slicers::SlicerCollection::Add(const PivotTable &pivot, int32_t row, int32_t column, const char16_t *baseFieldName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | const PivotTable\& | PivotTable object |
| row | int32_t | [Row](../../../aspose.cells/row/) index of the cell in the upper-left corner of the [Slicer](../../slicer/) range. |
| column | int32_t | [Column](../../../aspose.cells/column/) index of the cell in the upper-left corner of the [Slicer](../../slicer/) range. |
| baseFieldName | const char16_t* | The name of PivotField in PivotTable.BaseFields |
## ReturnValue
The new add [Slicer](../../slicer/) index
## Examples
```cpp
slicers.Add(pivotTable, 20, 12, u"fruit");
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* Class [SlicerCollection](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
## SlicerCollection::Add(const PivotTable\&, int32_t, int32_t, int32_t) method
Add a new [Slicer](../../slicer/) using PivotTable as data source.
```cpp
int32_t Aspose::Cells::Slicers::SlicerCollection::Add(const PivotTable &pivot, int32_t row, int32_t column, int32_t baseFieldIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | const PivotTable\& | PivotTable object |
| row | int32_t | [Row](../../../aspose.cells/row/) index of the cell in the upper-left corner of the [Slicer](../../slicer/) range. |
| column | int32_t | [Column](../../../aspose.cells/column/) index of the cell in the upper-left corner of the [Slicer](../../slicer/) range. |
| baseFieldIndex | int32_t | The index of PivotField in PivotTable.BaseFields |
## ReturnValue
The new add [Slicer](../../slicer/) index
## Examples
```cpp
slicers.Add(pivotTable, 20, 8, 0);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* Class [SlicerCollection](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
## SlicerCollection::Add(const PivotTable\&, const U16String\&, int32_t) method
Add a new [Slicer](../../slicer/) using PivotTable as data source.
```cpp
int32_t Aspose::Cells::Slicers::SlicerCollection::Add(const PivotTable &pivot, const U16String &destCellName, int32_t baseFieldIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | const PivotTable\& | PivotTable object |
| destCellName | const U16String\& | The cell in the upper-left corner of the [Slicer](../../slicer/) range. |
| baseFieldIndex | int32_t | The index of PivotField in PivotTable.BaseFields |
## ReturnValue
The new add [Slicer](../../slicer/) index
## Examples
```cpp
U16String val = u"E20";
slicers.Add(pivotTable, val, 0);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [SlicerCollection](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
## SlicerCollection::Add(const PivotTable\&, const char16_t*, int32_t) method
Add a new [Slicer](../../slicer/) using PivotTable as data source.
```cpp
int32_t Aspose::Cells::Slicers::SlicerCollection::Add(const PivotTable &pivot, const char16_t *destCellName, int32_t baseFieldIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | const PivotTable\& | PivotTable object |
| destCellName | const char16_t* | The cell in the upper-left corner of the [Slicer](../../slicer/) range. |
| baseFieldIndex | int32_t | The index of PivotField in PivotTable.BaseFields |
## ReturnValue
The new add [Slicer](../../slicer/) index
## Examples
```cpp
slicers.Add(pivotTable, u"E20", 0);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* Class [SlicerCollection](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
## SlicerCollection::Add(const PivotTable\&, int32_t, int32_t, const PivotField\&) method
Add a new [Slicer](../../slicer/) using PivotTable as data source.
```cpp
int32_t Aspose::Cells::Slicers::SlicerCollection::Add(const PivotTable &pivot, int32_t row, int32_t column, const PivotField &baseField)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | const PivotTable\& | PivotTable object |
| row | int32_t | [Row](../../../aspose.cells/row/) index of the cell in the upper-left corner of the [Slicer](../../slicer/) range. |
| column | int32_t | [Column](../../../aspose.cells/column/) index of the cell in the upper-left corner of the [Slicer](../../slicer/) range. |
| baseField | const PivotField\& | The PivotField in PivotTable.BaseFields |
## ReturnValue
The new add [Slicer](../../slicer/) index
## Examples
```cpp
slicers.Add(pivotTable, 3, 12, pivotTable.GetBaseFields().Get(0));
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* Class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* Class [SlicerCollection](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
## SlicerCollection::Add(const PivotTable\&, const U16String\&, const PivotField\&) method
Add a new [Slicer](../../slicer/) using PivotTable as data source.
```cpp
int32_t Aspose::Cells::Slicers::SlicerCollection::Add(const PivotTable &pivot, const U16String &destCellName, const PivotField &baseField)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | const PivotTable\& | PivotTable object |
| destCellName | const U16String\& | The cell in the upper-left corner of the [Slicer](../../slicer/) range. |
| baseField | const PivotField\& | The PivotField in PivotTable.BaseFields |
## ReturnValue
The new add [Slicer](../../slicer/) index
## Examples
```cpp
U16String val = u"I3";
slicers.Add(pivotTable, val, pivotTable.GetBaseFields().Get(0));
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* Class [SlicerCollection](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
## SlicerCollection::Add(const PivotTable\&, const char16_t*, const PivotField\&) method
Add a new [Slicer](../../slicer/) using PivotTable as data source.
```cpp
int32_t Aspose::Cells::Slicers::SlicerCollection::Add(const PivotTable &pivot, const char16_t *destCellName, const PivotField &baseField)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | const PivotTable\& | PivotTable object |
| destCellName | const char16_t* | The cell in the upper-left corner of the [Slicer](../../slicer/) range. |
| baseField | const PivotField\& | The PivotField in PivotTable.BaseFields |
## ReturnValue
The new add [Slicer](../../slicer/) index
## Examples
```cpp
slicers.Add(pivotTable, u"I3", pivotTable.GetBaseFields().Get(0));
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* Class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* Class [SlicerCollection](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
## SlicerCollection::Add(const ListObject\&, int32_t, const U16String\&) method
Add a new [Slicer](../../slicer/) using ListObjet as data source.
```cpp
int32_t Aspose::Cells::Slicers::SlicerCollection::Add(const ListObject &table, int32_t index, const U16String &destCellName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| table | const ListObject\& | ListObject object |
| index | int32_t | The index of ListColumn in ListObject.ListColumns |
| destCellName | const U16String\& | The cell in the upper-left corner of the [Slicer](../../slicer/) range. |
## ReturnValue
The new add [Slicer](../../slicer/) index
## Examples
```cpp
U16String val = u"E38";
slicers.Add(listTable, 1, val);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [ListObject](../../../aspose.cells.tables/listobject/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [SlicerCollection](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
## SlicerCollection::Add(const ListObject\&, int32_t, const char16_t*) method
Add a new [Slicer](../../slicer/) using ListObjet as data source.
```cpp
int32_t Aspose::Cells::Slicers::SlicerCollection::Add(const ListObject &table, int32_t index, const char16_t *destCellName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| table | const ListObject\& | ListObject object |
| index | int32_t | The index of ListColumn in ListObject.ListColumns |
| destCellName | const char16_t* | The cell in the upper-left corner of the [Slicer](../../slicer/) range. |
## ReturnValue
The new add [Slicer](../../slicer/) index
## Examples
```cpp
slicers.Add(listTable, 1, u"E38");
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [ListObject](../../../aspose.cells.tables/listobject/)
* Class [SlicerCollection](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
## SlicerCollection::Add(const ListObject\&, const ListColumn\&, const U16String\&) method
Add a new [Slicer](../../slicer/) using ListObjet as data source.
```cpp
int32_t Aspose::Cells::Slicers::SlicerCollection::Add(const ListObject &table, const ListColumn &listColumn, const U16String &destCellName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| table | const ListObject\& | ListObject object |
| listColumn | const ListColumn\& | The ListColumn in ListObject.ListColumns |
| destCellName | const U16String\& | The cell in the upper-left corner of the [Slicer](../../slicer/) range. |
## ReturnValue
The new add [Slicer](../../slicer/) index
## Examples
```cpp
U16String val = u"I38";
slicers.Add(listTable, listTable.GetListColumns().Get(1), val);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [ListObject](../../../aspose.cells.tables/listobject/)
* Class [ListColumn](../../../aspose.cells.tables/listcolumn/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [SlicerCollection](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
## SlicerCollection::Add(const ListObject\&, const ListColumn\&, const char16_t*) method
Add a new [Slicer](../../slicer/) using ListObjet as data source.
```cpp
int32_t Aspose::Cells::Slicers::SlicerCollection::Add(const ListObject &table, const ListColumn &listColumn, const char16_t *destCellName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| table | const ListObject\& | ListObject object |
| listColumn | const ListColumn\& | The ListColumn in ListObject.ListColumns |
| destCellName | const char16_t* | The cell in the upper-left corner of the [Slicer](../../slicer/) range. |
## ReturnValue
The new add [Slicer](../../slicer/) index
## Examples
```cpp
slicers.Add(listTable, listTable.GetListColumns().Get(1), u"I38");
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [ListObject](../../../aspose.cells.tables/listobject/)
* Class [ListColumn](../../../aspose.cells.tables/listcolumn/)
* Class [SlicerCollection](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
## SlicerCollection::Add(const ListObject\&, const ListColumn\&, int32_t, int32_t) method
Add a new [Slicer](../../slicer/) using ListObjet as data source.
```cpp
int32_t Aspose::Cells::Slicers::SlicerCollection::Add(const ListObject &table, const ListColumn &listColumn, int32_t row, int32_t column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| table | const ListObject\& | ListObject object |
| listColumn | const ListColumn\& | The ListColumn in ListObject.ListColumns |
| row | int32_t | [Row](../../../aspose.cells/row/) index of the cell in the upper-left corner of the [Slicer](../../slicer/) range. |
| column | int32_t | [Column](../../../aspose.cells/column/) index of the cell in the upper-left corner of the [Slicer](../../slicer/) range. |
## ReturnValue
The new add [Slicer](../../slicer/) index
## Examples
```cpp
slicers.Add(listTable, listTable.GetListColumns().Get(1), 38, 12);
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [ListObject](../../../aspose.cells.tables/listobject/)
* Class [ListColumn](../../../aspose.cells.tables/listcolumn/)
* Class [SlicerCollection](../)
* Namespace [Aspose::Cells::Slicers](../../)
* Library [Aspose.Cells for C++](../../../)
