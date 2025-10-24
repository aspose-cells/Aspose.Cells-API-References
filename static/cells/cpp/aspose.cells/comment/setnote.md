##Aspose::Cells::Comment::SetNote method
'Aspose::Cells::Comment::SetNote method. Represents the content of comment in C++.'
## Comment::SetNote(const U16String\&) method
Represents the content of comment.
```cpp
void Aspose::Cells::Comment::SetNote(const U16String &value)
```
## Remarks
If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment.
## Examples
```cpp
U16String note_1 = u"First note.";
U16String note_2 = u"Second note.";
comment1.SetNote(note_1);
comment2.SetNote(note_2);
```
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [Comment](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Comment::SetNote(const char16_t*) method
Represents the content of comment.
```cpp
void Aspose::Cells::Comment::SetNote(const char16_t *value)
```
## Remarks
If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment.
## Examples
```cpp
comment1.SetNote(u"First note.");
```
## See Also
* Class [Vector](../../vector/)
* Class [Comment](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
