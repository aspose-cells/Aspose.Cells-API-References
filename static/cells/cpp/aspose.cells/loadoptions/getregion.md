##Aspose::Cells::LoadOptions::GetRegion method
'Aspose::Cells::LoadOptions::GetRegion method. Gets or sets the regional settings used for the Workbook that will be loaded in C++.'
## LoadOptions::GetRegion method
Gets or sets the regional settings used for the [Workbook](../../workbook/) that will be loaded.
```cpp
CountryCode Aspose::Cells::LoadOptions::GetRegion()
```
## Remarks
The regional settings may be used for initializing some features for the workbook such as fonts, themes, and so on. For text based file formats, such as CSV, HTML, ..., the regional setting also will be used to detect number formats and parse text values to numeric or datetime values for cells. This setting will be kept for the instantiated workbook later, that is, WorkbookSettings.Region of the workbook will use the same region with this property.
## See Also
* Enum [CountryCode](../../countrycode/)
* Class [LoadOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
