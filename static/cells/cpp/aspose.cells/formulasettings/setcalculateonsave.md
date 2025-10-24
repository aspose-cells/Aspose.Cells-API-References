##Aspose::Cells::FormulaSettings::SetCalculateOnSave method
'Aspose::Cells::FormulaSettings::SetCalculateOnSave method. Indicates whether recalculate the workbook before saving the document, when in manual calculation mode in C++.'
## FormulaSettings::SetCalculateOnSave method
Indicates whether recalculate the workbook before saving the document, when in manual calculation mode.
```cpp
void Aspose::Cells::FormulaSettings::SetCalculateOnSave(bool value)
```
## Remarks
This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.
## See Also
* Class [Vector](../../vector/)
* Class [FormulaSettings](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
