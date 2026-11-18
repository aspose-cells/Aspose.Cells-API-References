---
title: "CommentCollection-klass"
linktitle: "CommentCollection"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "CommentCollection-klass. Inkapslar objektet som representerar commentcollection i Go."
type: docs
weight: 200
url: /sv/go-cpp/commentcollection/
---

## CommentCollection class

Inkapslar en samling av <see cref="Comment"/>‑objekt.

```go

type CommentCollection struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [AddThreadedComment_Int_Int_String_ThreadedCommentAuthor](./addthreadedcomment_int_int_string_threadedcommentauthor/) | Lägger till en trådad kommentar. |
| [AddThreadedComment_String_String_ThreadedCommentAuthor](./addthreadedcomment_string_string_threadedcommentauthor/) | Lägger till en trådad kommentar. |
| [GetThreadedComments_Int_Int](./getthreadedcomments_int_int/) | Hämtar de trådade kommentarerna efter rad- och kolumnindex. |
| [GetThreadedComments_String](./getthreadedcomments_string/) | Hämtar de trådade kommentarerna efter cellnamn. |
| [Add_Int_Int](./add_int_int/) | Lägger till en kommentar i samlingen. |
| [Add_String](./add_string/) | Lägger till en kommentar i samlingen. |
| [Get_Int](./get_int/) | Hämtar Comment‑elementet på det angivna indexet. |
| [Get_String](./get_string/) | Hämtar Comment‑elementet på den angivna cellen. |
| [Get_Int_Int](./get_int_int/) | Hämtar Comment‑elementet på det angivna radindexet och kolumnindexet. |
| [RemoveAt_String](./removeat_string/) | Tar bort kommentaren för den specifika cellen. |
| [RemoveAt_Int_Int](./removeat_int_int/) | Tar bort kommentaren för den specifika cellen. |
| [Clear](./clear/) | Tar bort alla kommentarer; |
| [GetCount](./getcount/) | Hämtar antalet element som finns i instansen. |
