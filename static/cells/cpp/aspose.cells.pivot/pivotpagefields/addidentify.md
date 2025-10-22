##Aspose::Cells::Pivot::PivotPageFields::AddIdentify method
'Aspose::Cells::Pivot::PivotPageFields::AddIdentify method. Sets which item label in each page field to use to identify the data range. The pageItemIndex.Length must be equal to PageFieldCount, so please add the page field first in C++.'
## PivotPageFields::AddIdentify method
Sets which item label in each page field to use to identify the data range. The pageItemIndex.Length must be equal to PageFieldCount, so please add the page field first.
```cpp
void Aspose::Cells::Pivot::PivotPageFields::AddIdentify(int32_t rangeIndex, const Vector<int32_t> &pageItemIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rangeIndex | int32_t | The consolidation data range index. |
| pageItemIndex | const Vector \<int32_t\>\& | The page item index in the each page field. pageItemIndex[2] = 1 means the second item in the third field to use to identify this range. pageItemIndex[1] = -1 means no item in the second field to use to identify this range and MS will auto create "blank" item in the second field to identify this range. |
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [PivotPageFields](../)
* Namespace [Aspose::Cells::Pivot](../../)
* Library [Aspose.Cells for C++](../../../)
