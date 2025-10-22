##Aspose::Cells::Pivot::PivotTable::CalculateData method
'Aspose::Cells::Pivot::PivotTable::CalculateData method. Calculates pivottable''s data to cells in C++.'
## PivotTable::CalculateData() method
Calculates pivottable's data to cells.
```cpp
void Aspose::Cells::Pivot::PivotTable::CalculateData()
```
## Remarks
Cell.Value in the pivot range could not return the correct result if the method is not been called. This method calculates data with an inner pivot cache,not original data source. So if the data source is changed, please call [RefreshData()](../refreshdata/) method first.
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTable](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
## PivotTable::CalculateData(const PivotTableCalculateOption\&) method
Calculating pivot tables with options.
```cpp
void Aspose::Cells::Pivot::PivotTable::CalculateData(const PivotTableCalculateOption &option)
```
| Parameter | Type | Description |
| --- | --- | --- |
| option | const PivotTableCalculateOption\& |  |
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotTableCalculateOption](../../pivottablecalculateoption/)
* Class [PivotTable](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
