##Aspose::Cells::LightCellsDataProvider::StartSheet method
'Aspose::Cells::LightCellsDataProvider::StartSheet method. Starts to save a worksheet in C++.'
## LightCellsDataProvider::StartSheet method
Starts to save a worksheet.
```cpp
virtual bool Aspose::Cells::LightCellsDataProvider::StartSheet(int32_t sheetIndex)=0
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | int32_t | index of current sheet to be saved. |
## ReturnValue
true if this provider will provide data for the given sheet; false if given sheet should use its normal data model(Cells).
## Remarks
It will be called at the beginning of saving a worksheet during saving a workbook. If the provider needs to refer to *## Examples
```cpp
sheetIndex
```
* later in startRow(Row) or startCell(Cell) method, that is, if the process needs to know which worksheet is being processed, the implementation should retain the *## Examples
```cpp
sheetIndex
```
* value here.
## See Also
* Class [Vector](../../vector/)
* Class [LightCellsDataProvider](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
