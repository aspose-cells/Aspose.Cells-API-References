---
title: "CommentCollection Sınıfı"
linktitle: "CommentCollection"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "CommentCollection sınıfı. Go'da commentcollection'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/commentcollection/
---

## CommentCollection class

<see cref="Comment"/> nesnelerinin bir koleksiyonunu kapsüller.

```go

type CommentCollection struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [AddThreadedComment_Int_Int_String_ThreadedCommentAuthor](./addthreadedcomment_int_int_string_threadedcommentauthor/) | Dallanmış bir yorum ekler. |
| [AddThreadedComment_String_String_ThreadedCommentAuthor](./addthreadedcomment_string_string_threadedcommentauthor/) | Dallanmış bir yorum ekler. |
| [GetThreadedComments_Int_Int](./getthreadedcomments_int_int/) | Satır ve sütun indeksine göre dallanmış yorumları alır. |
| [GetThreadedComments_String](./getthreadedcomments_string/) | Hücre adına göre dallanmış yorumları alır. |
| [Add_Int_Int](./add_int_int/) | Koleksiyona bir yorum ekler. |
| [Add_String](./add_string/) | Koleksiyona bir yorum ekler. |
| [Get_Int](./get_int/) | Belirtilen indeksteki Yorum öğesini alır. |
| [Get_String](./get_string/) | Belirtilen hücredeki Yorum öğesini alır. |
| [Get_Int_Int](./get_int_int/) | Belirtilen satır ve sütun indekslerindeki Yorum öğesini alır. |
| [RemoveAt_String](./removeat_string/) | Belirli hücrenin yorumunu kaldırır. |
| [RemoveAt_Int_Int](./removeat_int_int/) | Belirli hücrenin yorumunu kaldırır. |
| [Clear](./clear/) | Tüm yorumları kaldırır; |
| [GetCount](./getcount/) | Örnekte bulunan öğe sayısını alır. |
