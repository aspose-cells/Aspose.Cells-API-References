##Aspose::Cells::Row::SetIsHeightMatched method
'Aspose::Cells::Row::SetIsHeightMatched method. Indicates whether the row height matches current default font setting of the workbook. True of this property also denotes the row height is "automatic" without custom height value set by user in C++.'
## Row::SetIsHeightMatched method
Indicates whether the row height matches current default font setting of the workbook. True of this property also denotes the row height is "automatic" without custom height value set by user.
```cpp
void Aspose::Cells::Row::SetIsHeightMatched(bool value)
```
## Remarks
When this property is true, if the content in this row changes, generally the row height needs to be re-calculated(such as by [Worksheet.AutoFitRows()](../../worksheet/autofitrows/)) to get the same result with what is shown in ms excel when you opening the workbook in it.
## See Also
* Class [Vector](../../vector/)
* Class [Row](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
