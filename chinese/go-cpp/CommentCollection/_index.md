---
title: "CommentCollection 类"
linktitle: "CommentCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "CommentCollection 类。封装在 Go 中表示 commentcollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/commentcollection/
---

## CommentCollection class

封装 <see cref="Comment"/> 对象的集合。

```go

type CommentCollection struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [AddThreadedComment_Int_Int_String_ThreadedCommentAuthor](./addthreadedcomment_int_int_string_threadedcommentauthor/) | 添加一个线程评论。 |
| [AddThreadedComment_String_String_ThreadedCommentAuthor](./addthreadedcomment_string_string_threadedcommentauthor/) | 添加一个线程评论。 |
| [GetThreadedComments_Int_Int](./getthreadedcomments_int_int/) | 按行列索引获取线程评论。 |
| [GetThreadedComments_String](./getthreadedcomments_string/) | 按单元格名称获取线程评论。 |
| [Add_Int_Int](./add_int_int/) | 向集合中添加评论。 |
| [Add_String](./add_string/) | 向集合中添加评论。 |
| [Get_Int](./get_int/) | 获取指定索引处的 Comment 元素。 |
| [Get_String](./get_string/) | 获取指定单元格处的 Comment 元素。 |
| [Get_Int_Int](./get_int_int/) | 获取指定行索引和列索引处的 Comment 元素。 |
| [RemoveAt_String](./removeat_string/) | 移除特定单元格的评论。 |
| [RemoveAt_Int_Int](./removeat_int_int/) | 移除特定单元格的评论。 |
| [Clear](./clear/) | 移除所有评论； |
| [GetCount](./getcount/) | 获取实例中包含的元素数量。 |
