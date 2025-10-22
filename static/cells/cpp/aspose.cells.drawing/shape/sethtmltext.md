##Aspose::Cells::Drawing::Shape::SetHtmlText method
'Aspose::Cells::Drawing::Shape::SetHtmlText method. Gets and sets the html string which contains data and some formats in this textbox in C++.'
## Shape::SetHtmlText(const U16String\&) method
Gets and sets the html string which contains data and some formats in this textbox.
```cpp
void Aspose::Cells::Drawing::Shape::SetHtmlText(const U16String &value)
```
## Examples
```cpp
U16String txt = u"<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>";
U16String html = shape.GetHtmlText();
if (html.IsNull() || html.IsEmpty())
{
shape.SetHtmlText(txt);
}
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## Shape::SetHtmlText(const char16_t*) method
Gets and sets the html string which contains data and some formats in this textbox.
```cpp
void Aspose::Cells::Drawing::Shape::SetHtmlText(const char16_t *value)
```
## Examples
```cpp
U16String html = shape.GetHtmlText();
if (html.IsNull() || html.IsEmpty())
{
shape.SetHtmlText(u"<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>");
}
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
