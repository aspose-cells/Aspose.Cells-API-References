##Aspose::Cells::AutoFilter::AddFilter method
'Aspose::Cells::AutoFilter::AddFilter method. Adds a filter for a filter column in C++.'
## AutoFilter::AddFilter(int32_t, const U16String\&) method
Adds a filter for a filter column.
```cpp
void Aspose::Cells::AutoFilter::AddFilter(int32_t fieldIndex, const U16String &criteria)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int32_t | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| criteria | const U16String\& | The specified criteria (a string; for example, "101"). It only can be null or be one of the cells' value in this column. |
## Remarks
MS Excel 2007 supports multiple selection in a filter column.
## See Also
* Class [U16String](../../u16string/)
* Class [AutoFilter](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## AutoFilter::AddFilter(int32_t, const char16_t*) method
Adds a filter for a filter column.
```cpp
void Aspose::Cells::AutoFilter::AddFilter(int32_t fieldIndex, const char16_t *criteria)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int32_t | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| criteria | const char16_t* | The specified criteria (a string; for example, "101"). It only can be null or be one of the cells' value in this column. |
## Remarks
MS Excel 2007 supports multiple selection in a filter column.
## See Also
* Class [AutoFilter](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
