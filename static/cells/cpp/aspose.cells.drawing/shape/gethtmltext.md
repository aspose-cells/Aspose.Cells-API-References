##Aspose::Cells::Drawing::Shape::GetHtmlText method
'Aspose::Cells::Drawing::Shape::GetHtmlText method. Gets and sets the html string which contains data and some formats in this textbox in C++.'
## Shape::GetHtmlText method
Gets and sets the html string which contains data and some formats in this textbox.
```cpp
U16String Aspose::Cells::Drawing::Shape::GetHtmlText()
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
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
