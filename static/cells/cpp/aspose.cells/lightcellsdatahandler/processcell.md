##Aspose::Cells::LightCellsDataHandler::ProcessCell method
'Aspose::Cells::LightCellsDataHandler::ProcessCell method. Starts to process one cell in C++.'
## LightCellsDataHandler::ProcessCell method
Starts to process one cell.
```cpp
virtual bool Aspose::Cells::LightCellsDataHandler::ProcessCell(Cell &cell)=0
```
| Parameter | Type | Description |
| --- | --- | --- |
| cell | Cell\& | [Cell](../../cell/) object which is being processed currently |
## ReturnValue
whether this cell needs to be kept in cells model of current sheet. Commonly it should be false so that all cells will not be kept in memory after being processed and then memory be saved. For some special purpose such as user needs to access some cells later after the whole workbook having been processed, user can make this method return true to keep those special cells in [Cells](../../cells/) model and access them later by APIs such as [Cells](../../cells/)[row, column]. However, keeping cells data in [Cells](../../cells/) model will requires more memory and if all cells are kept then reading template file in LightCells mode will become same with reading it in normal way.
## Remarks
It will be called after one cell's data has been read.
## See Also
* Class [Vector](../../vector/)
* Class [Cell](../../cell/)
* Class [LightCellsDataHandler](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
