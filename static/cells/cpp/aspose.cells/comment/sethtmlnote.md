##Aspose::Cells::Comment::SetHtmlNote method
'Aspose::Cells::Comment::SetHtmlNote method. Gets and sets the html string which contains data and some formats in this comment in C++.'
## Comment::SetHtmlNote(const U16String\&) method
Gets and sets the html string which contains data and some formats in this comment.
```cpp
void Aspose::Cells::Comment::SetHtmlNote(const U16String &value)
```
## Remarks
If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment.
## Examples
```cpp
U16String htmlNote = u"<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>";
comment1.SetHtmlNote(htmlNote);
```
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [Comment](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Comment::SetHtmlNote(const char16_t*) method
Gets and sets the html string which contains data and some formats in this comment.
```cpp
void Aspose::Cells::Comment::SetHtmlNote(const char16_t *value)
```
## Remarks
If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment.
## Examples
```cpp
comment1.SetHtmlNote(u"<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>");
```
## See Also
* Class [Vector](../../vector/)
* Class [Comment](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
