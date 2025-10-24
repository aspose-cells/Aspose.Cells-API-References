##Aspose::Cells::CommentCollection::Get method
'Aspose::Cells::CommentCollection::Get method. Gets the Comment element at the specified index in C++.'
## CommentCollection::Get(int32_t) method
Gets the [Comment](../../comment/) element at the specified index.
```cpp
Comment Aspose::Cells::CommentCollection::Get(int32_t index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | int32_t | The zero based index of the element. |
## ReturnValue
The element at the specified index.
## Examples
```cpp
Comment comment3 = comments.Get(0);
comment3.SetNote(u"Three note.");
```
## See Also
* Class [Comment](../../comment/)
* Class [Vector](../../vector/)
* Class [CommentCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## CommentCollection::Get(const U16String\&) method
Gets the [Comment](../../comment/) element at the specified cell.
```cpp
Comment Aspose::Cells::CommentCollection::Get(const U16String &cellName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | const U16String\& | [Cell](../../cell/) name. |
## ReturnValue
The element at the specified cell.
## Examples
```cpp
U16String val = u"B2";
Comment comment4 = comments.Get(val);
comment4.SetNote(u"Four note.");
```
## See Also
* Class [Comment](../../comment/)
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [CommentCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## CommentCollection::Get(const char16_t*) method
Gets the [Comment](../../comment/) element at the specified cell.
```cpp
Comment Aspose::Cells::CommentCollection::Get(const char16_t *cellName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | const char16_t* | [Cell](../../cell/) name. |
## ReturnValue
The element at the specified cell.
## Examples
```cpp
Comment comment4 = comments.Get(u"B2");
comment4.SetNote(u"Four note.");
```
## See Also
* Class [Comment](../../comment/)
* Class [Vector](../../vector/)
* Class [CommentCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## CommentCollection::Get(int32_t, int32_t) method
Gets the [Comment](../../comment/) element at the specified row index and column index.
```cpp
Comment Aspose::Cells::CommentCollection::Get(int32_t row, int32_t column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | int32_t | [Row](../../row/) index. |
| column | int32_t | [Column](../../column/) index. |
## ReturnValue
The element at the specified cell.
## Examples
```cpp
Comment comment5 = comments.Get(1, 1);
comment5.SetNote(u"Five note.");
```
## See Also
* Class [Comment](../../comment/)
* Class [Vector](../../vector/)
* Class [CommentCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
