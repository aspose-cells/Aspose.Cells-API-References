##Aspose::Cells::WorkbookSettings::GetShowTabs method
'Aspose::Cells::WorkbookSettings::GetShowTabs method. Get or sets a value whether the Workbook tabs are displayed in C++.'
## WorkbookSettings::GetShowTabs method
Get or sets a value whether the [Workbook](../../workbook/) tabs are displayed.
```cpp
bool Aspose::Cells::WorkbookSettings::GetShowTabs()
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
