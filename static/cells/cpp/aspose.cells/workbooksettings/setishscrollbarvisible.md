##Aspose::Cells::WorkbookSettings::SetIsHScrollBarVisible method
'Aspose::Cells::WorkbookSettings::SetIsHScrollBarVisible method. Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar in C++.'
## WorkbookSettings::SetIsHScrollBarVisible method
Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar.
```cpp
void Aspose::Cells::WorkbookSettings::SetIsHScrollBarVisible(bool value)
```
## Remarks
The default value is true.
## Examples
```cpp
//The following code makes the horizontal scroll bar invisible for the spreadsheet.
// Hide the horizontal scroll bar of the Excel file.
if (settings.IsHScrollBarVisible())
{
settings.SetIsHScrollBarVisible(false);
}
```
## See Also
* Class [Vector](../../vector/)
* Class [WorkbookSettings](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
