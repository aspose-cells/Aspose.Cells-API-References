##Aspose::Cells::LightCellsDataHandler::StartCell method
'Aspose::Cells::LightCellsDataHandler::StartCell method. Prepares to process a cell in C++.'
## LightCellsDataHandler::StartCell method
Prepares to process a cell.
```cpp
virtual bool Aspose::Cells::LightCellsDataHandler::StartCell(int32_t columnIndex)=0
```
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | int32_t | column index of the cell to be processed |
## ReturnValue
whether this cell needs to be processed. false to ignore the cell and check the next one until reach the end of cells data of current row
## Remarks
It will be called when reaching an existing cell in current row. Current row is the row of last call of ProcessRow(Row).
## See Also
* Class [Vector](../../vector/)
* Class [LightCellsDataHandler](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
