##Aspose::Cells::CommentCollection class
'Aspose::Cells::CommentCollection class. Encapsulates a collection of Comment objects in C++.'
## CommentCollection class
Encapsulates a collection of [Comment](../comment/) objects.
```cpp
class CommentCollection
```
## Methods
| Method | Description |
| --- | --- |
| [Add(int32_t row, int32_t column)](./add/) | Adds a comment to the collection. |
| [Add(const U16String\& cellName)](./add/) | Adds a comment to the collection. |
| [Add(const char16_t* cellName)](./add/) | Adds a comment to the collection. |
| [AddThreadedComment(int32_t row, int32_t column, const U16String\& text, const ThreadedCommentAuthor\& author)](./addthreadedcomment/) | Adds a threaded comment. |
| [AddThreadedComment(int32_t row, int32_t column, const char16_t* text, const ThreadedCommentAuthor\& author)](./addthreadedcomment/) | Adds a threaded comment. |
| [AddThreadedComment(const U16String\& cellName, const U16String\& text, const ThreadedCommentAuthor\& author)](./addthreadedcomment/) | Adds a threaded comment. |
| [AddThreadedComment(const char16_t* cellName, const char16_t* text, const ThreadedCommentAuthor\& author)](./addthreadedcomment/) | Adds a threaded comment. |
| [Clear()](./clear/) | Removes all comments;. |
| [CommentCollection(CommentCollection_Impl* impl)](./commentcollection/) | Constructs from an implementation object. |
| [CommentCollection(const CommentCollection\& src)](./commentcollection/) | Copy constructor. |
| [Get(int32_t index)](./get/) | Gets the [Comment](../comment/) element at the specified index. |
| [Get(const U16String\& cellName)](./get/) | Gets the [Comment](../comment/) element at the specified cell. |
| [Get(const char16_t* cellName)](./get/) | Gets the [Comment](../comment/) element at the specified cell. |
| [Get(int32_t row, int32_t column)](./get/) | Gets the [Comment](../comment/) element at the specified row index and column index. |
| [GetCount()](./getcount/) |  |
| [GetThreadedComments(int32_t row, int32_t column)](./getthreadedcomments/) | Gets the threaded comments by row and column index. |
| [GetThreadedComments(const U16String\& cellName)](./getthreadedcomments/) | Gets the threaded comments by cell name. |
| [GetThreadedComments(const char16_t* cellName)](./getthreadedcomments/) | Gets the threaded comments by cell name. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const CommentCollection\& src)](./operator_asm/) | operator= |
| [RemoveAt(const U16String\& cellName)](./removeat/) | Removes the comment of the specific cell. |
| [RemoveAt(const char16_t* cellName)](./removeat/) | Removes the comment of the specific cell. |
| [RemoveAt(int32_t row, int32_t column)](./removeat/) | Removes the comment of the specific cell. |
| [~CommentCollection()](./~commentcollection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
CommentCollection comments = workbook.GetWorksheets().Get(0).GetComments();
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
