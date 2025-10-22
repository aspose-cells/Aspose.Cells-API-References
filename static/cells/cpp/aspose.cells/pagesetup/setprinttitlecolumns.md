##Aspose::Cells::PageSetup::SetPrintTitleColumns method
'Aspose::Cells::PageSetup::SetPrintTitleColumns method. Represents the columns that contain the cells to be repeated on the left side of each page in C++.'
## PageSetup::SetPrintTitleColumns(const U16String\&) method
Represents the columns that contain the cells to be repeated on the left side of each page.
```cpp
void Aspose::Cells::PageSetup::SetPrintTitleColumns(const U16String &value)
```
## Examples
```cpp
U16String val = u"$A:$A";
if (pageSetup.GetPrintTitleColumns().IsNull())
{
pageSetup.SetPrintTitleColumns(val);
}
```
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [PageSetup](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## PageSetup::SetPrintTitleColumns(const char16_t*) method
Represents the columns that contain the cells to be repeated on the left side of each page.
```cpp
void Aspose::Cells::PageSetup::SetPrintTitleColumns(const char16_t *value)
```
## Examples
```cpp
if (pageSetup.GetPrintTitleColumns().IsNull())
{
pageSetup.SetPrintTitleColumns(u"$A:$A");
}
```
## See Also
* Class [Vector](../../vector/)
* Class [PageSetup](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
