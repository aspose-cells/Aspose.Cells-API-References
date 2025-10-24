##Aspose::Cells::CommentCollection::GetThreadedComments method
'Aspose::Cells::CommentCollection::GetThreadedComments method. Gets the threaded comments by row and column index in C++.'
## CommentCollection::GetThreadedComments(int32_t, int32_t) method
Gets the threaded comments by row and column index.
```cpp
ThreadedCommentCollection Aspose::Cells::CommentCollection::GetThreadedComments(int32_t row, int32_t column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | int32_t | The row index. |
| column | int32_t | The column index. |
## ReturnValue
## Examples
```cpp
ThreadedCommentCollection threadedComments1 = comments.GetThreadedComments(1, 1);
for (int i = 0; i < threadedComments1.GetCount(); ++i)
{
ThreadedComment tc = threadedComments1.Get(i);
U16String note = tc.GetNotes();
}
```
## See Also
* Class [ThreadedCommentCollection](../../threadedcommentcollection/)
* Class [Vector](../../vector/)
* Class [CommentCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## CommentCollection::GetThreadedComments(const U16String\&) method
Gets the threaded comments by cell name.
```cpp
ThreadedCommentCollection Aspose::Cells::CommentCollection::GetThreadedComments(const U16String &cellName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | const U16String\& | The name of the cell. |
## ReturnValue
## Examples
```cpp
U16String comt = u"B2";
ThreadedCommentCollection threadedComments2 = comments.GetThreadedComments(comt);
for (int i = 0; i < threadedComments2.GetCount(); ++i)
{
ThreadedComment tc = threadedComments2.Get(i);
U16String note = tc.GetNotes();
}
```
## See Also
* Class [ThreadedCommentCollection](../../threadedcommentcollection/)
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [CommentCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## CommentCollection::GetThreadedComments(const char16_t*) method
Gets the threaded comments by cell name.
```cpp
ThreadedCommentCollection Aspose::Cells::CommentCollection::GetThreadedComments(const char16_t *cellName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | const char16_t* | The name of the cell. |
## ReturnValue
## Examples
```cpp
ThreadedCommentCollection threadedComments2 = comments.GetThreadedComments(u"B2");
for (int i = 0; i < threadedComments2.GetCount(); ++i)
{
ThreadedComment tc = threadedComments2.Get(i);
U16String note = tc.GetNotes();
}
```
## See Also
* Class [ThreadedCommentCollection](../../threadedcommentcollection/)
* Class [Vector](../../vector/)
* Class [CommentCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
