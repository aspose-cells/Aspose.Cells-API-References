---
title: "فئة CommentCollection"
linktitle: "CommentCollection"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة CommentCollection. تغلف الكائن الذي يمثل commentcollection في Go."
type: docs
weight: 200
url: /ar/go-cpp/commentcollection/
---

## CommentCollection class

يغلف مجموعة من كائنات <see cref="Comment"/>.

```go

type CommentCollection struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [AddThreadedComment_Int_Int_String_ThreadedCommentAuthor](./addthreadedcomment_int_int_string_threadedcommentauthor/) | يضيف تعليقًا متسلسلًا. |
| [AddThreadedComment_String_String_ThreadedCommentAuthor](./addthreadedcomment_string_string_threadedcommentauthor/) | يضيف تعليقًا متسلسلًا. |
| [GetThreadedComments_Int_Int](./getthreadedcomments_int_int/) | يحصل على التعليقات المتسلسلة حسب فهرس الصف والعمود. |
| [GetThreadedComments_String](./getthreadedcomments_string/) | يحصل على التعليقات المتسلسلة حسب اسم الخلية. |
| [Add_Int_Int](./add_int_int/) | يضيف تعليقًا إلى المجموعة. |
| [Add_String](./add_string/) | يضيف تعليقًا إلى المجموعة. |
| [Get_Int](./get_int/) | يحصل على عنصر التعليق في الفهرس المحدد. |
| [Get_String](./get_string/) | يحصل على عنصر التعليق في الخلية المحددة. |
| [Get_Int_Int](./get_int_int/) | يحصل على عنصر التعليق في فهرس الصف والعمود المحددين. |
| [RemoveAt_String](./removeat_string/) | يزيل التعليق الخاص بالخلية المحددة. |
| [RemoveAt_Int_Int](./removeat_int_int/) | يزيل التعليق الخاص بالخلية المحددة. |
| [Clear](./clear/) | يزيل جميع التعليقات؛ |
| [GetCount](./getcount/) | يحصل على عدد العناصر الموجودة في المثيل. |
