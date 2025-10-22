##Aspose::Cells::LightCellsDataProvider::StartCell method
'Aspose::Cells::LightCellsDataProvider::StartCell method. Starts to save data of one cell in C++.'
## LightCellsDataProvider::StartCell method
Starts to save data of one cell.
```cpp
virtual void Aspose::Cells::LightCellsDataProvider::StartCell(Cell &cell)=0
```
| Parameter | Type | Description |
| --- | --- | --- |
| cell | Cell\& | [Cell](../../cell/) object for implementation to fill data. Its column index is the returned value of latest call of [NextCell()](../nextcell/). If the cell has been initialized in the inner cells model, the existed cell object will be used. Otherwise a temporary [Cell](../../cell/) object will be used for implementation to fill data. |
## See Also
* Class [Vector](../../vector/)
* Class [Cell](../../cell/)
* Class [LightCellsDataProvider](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
