##Aspose::Cells::WorkbookSettings::SetRegion method
'Aspose::Cells::WorkbookSettings::SetRegion method. Gets or sets the regional settings for workbook in C++.'
## WorkbookSettings::SetRegion method
Gets or sets the regional settings for workbook.
```cpp
void Aspose::Cells::WorkbookSettings::SetRegion(CountryCode value)
```
## Remarks
1. Regional settings used by [Aspose.Cells](../../) component for a workbook loaded from template file: i). For an XLS file, there are fields defined for regional settings and MS Excel does save regional settings data into the file when saving the XLS file. So, we use the saved region in the template file for the workbook. If you do not want to use the region saved in the XLS file, please reset it to the expected one (such as, [CountryCode.Default](../../countrycode/)) after loading the template file. And, we save the user specified value (by this method) into the file too when saving an XLS file. ii). For other file formats, such as, XLSX, XLSB...etc., there is no field defined for regional settings in the file format specification. So, we use the regional settings of application's environment for the workbook. And, the user specified value (by this method) cannot be kept for the generated files with those file formats.
1. For the view effect in MS Excel: The applied regional settings here can take effect only at runtime with [Aspose.Cells](../../) component and not when viewing the generated file with MS Excel. Even for the generated XLS file in which the specified regional settings data has been saved, when viewing/editing it with MS Excel, the used region to perform formatting by MS Excel is always the default regional settings of the environment where MS Excel is running, not the one saved in the file. It is MS Excel's behavior and cannot be changed by code.
## See Also
* Class [Vector](../../vector/)
* Enum [CountryCode](../../countrycode/)
* Class [WorkbookSettings](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
