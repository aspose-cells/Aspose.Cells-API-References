##Aspose::Cells::CommentCollection::RemoveAt method
'Aspose::Cells::CommentCollection::RemoveAt method. Removes the comment of the specific cell in C++.'
## CommentCollection::RemoveAt(const U16String\&) method
Removes the comment of the specific cell.
```cpp
void Aspose::Cells::CommentCollection::RemoveAt(const U16String &cellName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | const U16String\& | The name of cell which contains a comment. |
## Examples
```cpp
U16String val = u"B2";
comments.RemoveAt(val);
```
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [CommentCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## CommentCollection::RemoveAt(const char16_t*) method
Removes the comment of the specific cell.
```cpp
void Aspose::Cells::CommentCollection::RemoveAt(const char16_t *cellName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | const char16_t* | The name of cell which contains a comment. |
## Examples
```cpp
comments.RemoveAt(u"B2");
```
## See Also
* Class [Vector](../../vector/)
* Class [CommentCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## CommentCollection::RemoveAt(int32_t, int32_t) method
Removes the comment of the specific cell.
```cpp
void Aspose::Cells::CommentCollection::RemoveAt(int32_t row, int32_t column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | int32_t | The row index. |
| column | int32_t | the column index. |
## Examples
```cpp
comments.RemoveAt(1, 1);
```
## See Also
* Class [Vector](../../vector/)
* Class [CommentCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
