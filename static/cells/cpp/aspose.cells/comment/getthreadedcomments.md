##Aspose::Cells::Comment::GetThreadedComments method
'Aspose::Cells::Comment::GetThreadedComments method. Gets the list of threaded comments; in C++.'
## Comment::GetThreadedComments method
Gets the list of threaded comments;.
```cpp
ThreadedCommentCollection Aspose::Cells::Comment::GetThreadedComments()
```
## Examples
```cpp
ThreadedCommentCollection threadedComments = comment1.GetThreadedComments();
for (int i = 0; i < threadedComments.GetCount(); ++i)
{
ThreadedComment tc = threadedComments.Get(i);
U16String note = tc.GetNotes();
}
```
## See Also
* Class [ThreadedCommentCollection](../../threadedcommentcollection/)
* Class [Comment](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
