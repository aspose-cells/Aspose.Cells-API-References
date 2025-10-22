##Aspose::Cells::Cells::Subtotal method
'Aspose::Cells::Cells::Subtotal method. Creates subtotals for the range in C++.'
## Cells::Subtotal(const CellArea\&, int32_t, ConsolidationFunction, const Vector \<int32_t\>\&) method
Creates subtotals for the range.
```cpp
void Aspose::Cells::Cells::Subtotal(const CellArea &ca, int32_t groupBy, ConsolidationFunction function, const Vector<int32_t> &totalList)
```
| Parameter | Type | Description |
| --- | --- | --- |
| ca | const CellArea\& | The range |
| groupBy | int32_t | The field to group by, as a zero-based integer offset |
| function | ConsolidationFunction | The subtotal function. |
| totalList | const Vector \<int32_t\>\& | An array of zero-based field offsets, indicating the fields to which the subtotals are added. |
## See Also
* Class [Vector](../../vector/)
* Class [CellArea](../../cellarea/)
* Enum [ConsolidationFunction](../../consolidationfunction/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cells::Subtotal(const CellArea\&, int32_t, ConsolidationFunction, const Vector \<int32_t\>\&, bool, bool, bool) method
Creates subtotals for the range.
```cpp
void Aspose::Cells::Cells::Subtotal(const CellArea &ca, int32_t groupBy, ConsolidationFunction function, const Vector<int32_t> &totalList, bool replace, bool pageBreaks, bool summaryBelowData)
```
| Parameter | Type | Description |
| --- | --- | --- |
| ca | const CellArea\& | The range |
| groupBy | int32_t | The field to group by, as a zero-based integer offset |
| function | ConsolidationFunction | The subtotal function. |
| totalList | const Vector \<int32_t\>\& | An array of zero-based field offsets, indicating the fields to which the subtotals are added. |
| replace | bool | Indicates whether replace the current subtotals |
| pageBreaks | bool | Indicates whether add page break between groups |
| summaryBelowData | bool | Indicates whether add summary below data. |
## See Also
* Class [Vector](../../vector/)
* Class [CellArea](../../cellarea/)
* Enum [ConsolidationFunction](../../consolidationfunction/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
