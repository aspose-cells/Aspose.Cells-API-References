##Aspose::Cells::Cell::GetNumberCategoryType method
'Aspose::Cells::Cell::GetNumberCategoryType method. Represents the category type of this cell''s number formatting in C++.'
## Cell::GetNumberCategoryType method
Represents the category type of this cell's number formatting.
```cpp
NumberCategoryType Aspose::Cells::Cell::GetNumberCategoryType()
```
## Remarks
When cell's formatting pattern is combined with conditional formatting patterns, then the returned type is corresponding to the part which is used for current value of this cell. For example, if the formatting pattern for this cell is "#,##0;(#,##0);"-";@", then when cell's value is numeric and not 0, the returned type is [NumberCategoryType.Number](../../numbercategorytype/); When cell's value is 0 or not numeric value, the returned type is [NumberCategoryType.Text](../../numbercategorytype/).
## See Also
* Enum [NumberCategoryType](../../numbercategorytype/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
