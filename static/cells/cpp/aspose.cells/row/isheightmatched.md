##Aspose::Cells::Row::IsHeightMatched method
'Aspose::Cells::Row::IsHeightMatched method. Indicates whether the row height matches current default font setting of the workbook. True of this property also denotes the row height is "automatic" without custom height value set by user in C++.'
## Row::IsHeightMatched method
Indicates whether the row height matches current default font setting of the workbook. True of this property also denotes the row height is "automatic" without custom height value set by user.
```cpp
bool Aspose::Cells::Row::IsHeightMatched()
```
## Remarks
When this property is true, if the content in this row changes, generally the row height needs to be re-calculated(such as by [Worksheet.AutoFitRows()](../../worksheet/autofitrows/)) to get the same result with what is shown in ms excel when you opening the workbook in it.
## See Also
* Class [Vector](../../vector/)
* Class [Row](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
