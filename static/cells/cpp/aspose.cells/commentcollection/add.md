##Aspose::Cells::CommentCollection::Add method
'Aspose::Cells::CommentCollection::Add method. Adds a comment to the collection in C++.'
## CommentCollection::Add(int32_t, int32_t) method
Adds a comment to the collection.
```cpp
int32_t Aspose::Cells::CommentCollection::Add(int32_t row, int32_t column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | int32_t | [Cell](../../cell/) row index. |
| column | int32_t | [Cell](../../cell/) column index. |
## ReturnValue
[Comment](../../comment/) object index.
## Examples
```cpp
int commentIndex1 = comments.Add(0, 0);
Comment comment1 = comments.Get(commentIndex1);
comment1.SetNote(u"First note.");
comment1.GetFont().SetName(u"Times New Roman");
```
## See Also
* Class [Vector](../../vector/)
* Class [CommentCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## CommentCollection::Add(const U16String\&) method
Adds a comment to the collection.
```cpp
int32_t Aspose::Cells::CommentCollection::Add(const U16String &cellName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | const U16String\& | [Cell](../../cell/) name. |
## ReturnValue
[Comment](../../comment/) object index.
## Examples
```cpp
U16String val = u"B2";
int commentIndex2 = comments.Add(val);
Comment comment2 = comments.Get(commentIndex2);
comment2.SetNote(u"Second note.");
comment2.GetFont().SetName(u"Times New Roman");
```
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [CommentCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## CommentCollection::Add(const char16_t*) method
Adds a comment to the collection.
```cpp
int32_t Aspose::Cells::CommentCollection::Add(const char16_t *cellName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | const char16_t* | [Cell](../../cell/) name. |
## ReturnValue
[Comment](../../comment/) object index.
## Examples
```cpp
int commentIndex2 = comments.Add(u"B2");
Comment comment2 = comments.Get(commentIndex2);
comment2.SetNote(u"Second note.");
comment2.GetFont().SetName(u"Times New Roman");
```
## See Also
* Class [Vector](../../vector/)
* Class [CommentCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
