##Aspose::Cells::PageSetup::SetPrintTitleRows method
'Aspose::Cells::PageSetup::SetPrintTitleRows method. Represents the rows that contain the cells to be repeated at the top of each page in C++.'
## PageSetup::SetPrintTitleRows(const U16String\&) method
Represents the rows that contain the cells to be repeated at the top of each page.
```cpp
void Aspose::Cells::PageSetup::SetPrintTitleRows(const U16String &value)
```
## Examples
```cpp
U16String val = u"$1:$1";
if (pageSetup.GetPrintTitleRows().IsNull())
{
pageSetup.SetPrintTitleRows(val);
}
```
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [PageSetup](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## PageSetup::SetPrintTitleRows(const char16_t*) method
Represents the rows that contain the cells to be repeated at the top of each page.
```cpp
void Aspose::Cells::PageSetup::SetPrintTitleRows(const char16_t *value)
```
## Examples
```cpp
if (pageSetup.GetPrintTitleRows().IsNull())
{
pageSetup.SetPrintTitleRows(u"$1:$1");
}
```
## See Also
* Class [Vector](../../vector/)
* Class [PageSetup](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
