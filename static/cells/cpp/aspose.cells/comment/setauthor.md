##Aspose::Cells::Comment::SetAuthor method
'Aspose::Cells::Comment::SetAuthor method. Gets and sets Name of the original comment author in C++.'
## Comment::SetAuthor(const U16String\&) method
Gets and sets [Name](../../name/) of the original comment author.
```cpp
void Aspose::Cells::Comment::SetAuthor(const U16String &value)
```
## Examples
```cpp
if (comment1.GetAuthor().IsNull())
{
U16String author = u"Carl.Yang";
comment1.SetAuthor(author);
}
```
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [Comment](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Comment::SetAuthor(const char16_t*) method
Gets and sets [Name](../../name/) of the original comment author.
```cpp
void Aspose::Cells::Comment::SetAuthor(const char16_t *value)
```
## Examples
```cpp
if (comment1.GetAuthor().IsNull())
{
comment1.SetAuthor(u"Carl.Yang");
}
```
## See Also
* Class [Vector](../../vector/)
* Class [Comment](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
