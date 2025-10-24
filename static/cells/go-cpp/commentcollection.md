##CommentCollection Class
'CommentCollection class. Encapsulates the object that represents commentcollection in Go.'
## CommentCollection class
Encapsulates a collection of <see cref="Comment"/> objects.
```go
type CommentCollection struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[AddThreadedComment_Int_Int_String_ThreadedCommentAuthor](./addthreadedcomment_int_int_string_threadedcommentauthor/) | Adds a threaded comment. |
|[AddThreadedComment_String_String_ThreadedCommentAuthor](./addthreadedcomment_string_string_threadedcommentauthor/) | Adds a threaded comment. |
|[GetThreadedComments_Int_Int](./getthreadedcomments_int_int/) | Gets the threaded comments by row and column index. |
|[GetThreadedComments_String](./getthreadedcomments_string/) | Gets the threaded comments by cell name. |
|[Add_Int_Int](./add_int_int/) | Adds a comment to the collection. |
|[Add_String](./add_string/) | Adds a comment to the collection. |
|[Get_Int](./get_int/) | Gets the Comment element at the specified index. |
|[Get_String](./get_string/) | Gets the Comment element at the specified cell. |
|[Get_Int_Int](./get_int_int/) | Gets the Comment element at the specified row index and column index. |
|[RemoveAt_String](./removeat_string/) | Removes the comment of the specific cell. |
|[RemoveAt_Int_Int](./removeat_int_int/) | Removes the comment of the specific cell. |
|[Clear](./clear/) | Removes all comments; |
|[GetCount](./getcount/) |  |
