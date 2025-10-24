##Aspose::Cells::LightCellsDataProvider::StartRow method
'Aspose::Cells::LightCellsDataProvider::StartRow method. Starts to save data of one row in C++.'
## LightCellsDataProvider::StartRow method
Starts to save data of one row.
```cpp
virtual void Aspose::Cells::LightCellsDataProvider::StartRow(Row &row)=0
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Row\& | [Row](../../row/) object for implementation to fill data. Its row index is the returned value of latest call of [NextRow()](../nextrow/). If the row has been initialized in the inner cells model, the existing row object will be used. Otherwise a temporary [Row](../../row/) object will be used for implementation to fill data. |
## Remarks
It will be called at the beginning of saving a row and its cells data. If current row has some custom properties such as height, style, ...etc., implementation should set those properties to given [Row](../../row/) object here.
## See Also
* Class [Vector](../../vector/)
* Class [Row](../../row/)
* Class [LightCellsDataProvider](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
