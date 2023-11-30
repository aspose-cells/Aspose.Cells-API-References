---
title: Aspose::Cells::Comment::GetThreadedComments method
linktitle: GetThreadedComments
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Comment::GetThreadedComments method. Gets the list of threaded comments; in C++.'
type: docs
weight: 1200
url: /cpp/aspose.cells/comment/getthreadedcomments/
---
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
