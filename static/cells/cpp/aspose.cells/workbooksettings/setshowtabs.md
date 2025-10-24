##Aspose::Cells::WorkbookSettings::SetShowTabs method
'Aspose::Cells::WorkbookSettings::SetShowTabs method. Get or sets a value whether the Workbook tabs are displayed in C++.'
## WorkbookSettings::SetShowTabs method
Get or sets a value whether the [Workbook](../../workbook/) tabs are displayed.
```cpp
void Aspose::Cells::WorkbookSettings::SetShowTabs(bool value)
```
## Remarks
The default value is true.
## Examples
```cpp
// Hide the spreadsheet tabs.
if (workbook.GetSettings().GetShowTabs())
{
workbook.GetSettings().SetShowTabs(false);
}
```
## See Also
* Class [Vector](../../vector/)
* Class [WorkbookSettings](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
