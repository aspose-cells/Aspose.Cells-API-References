##Aspose::Cells::FormulaSettings::SetCalculationId method
'Aspose::Cells::FormulaSettings::SetCalculationId method. Specifies the version of the calculation engine used to calculate values in the workbook in C++.'
## FormulaSettings::SetCalculationId(const U16String\&) method
Specifies the version of the calculation engine used to calculate values in the workbook.
```cpp
void Aspose::Cells::FormulaSettings::SetCalculationId(const U16String &value)
```
## Remarks
This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. In the case of ms excel, if the value of this property is less than the recalculation engine identifier associated with the application that opens the resultant file, the application will recalculate the results of all formulas on this workbook immediately after loading the file. For performance consideration for most users' applications, we do not calculate any formula on the workbook automatically, no matter what value has been set for this property.
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [FormulaSettings](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## FormulaSettings::SetCalculationId(const char16_t*) method
Specifies the version of the calculation engine used to calculate values in the workbook.
```cpp
void Aspose::Cells::FormulaSettings::SetCalculationId(const char16_t *value)
```
## Remarks
This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. In the case of ms excel, if the value of this property is less than the recalculation engine identifier associated with the application that opens the resultant file, the application will recalculate the results of all formulas on this workbook immediately after loading the file. For performance consideration for most users' applications, we do not calculate any formula on the workbook automatically, no matter what value has been set for this property.
## See Also
* Class [Vector](../../vector/)
* Class [FormulaSettings](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
