---
title: "Класс CommentCollection"
linktitle: "CommentCollection"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс CommentCollection. Инкапсулирует объект, представляющий commentcollection в Go."
type: docs
weight: 200
url: /ru/go-cpp/commentcollection/
---

## CommentCollection class

Инкапсулирует коллекцию объектов <see cref="Comment"/>.

```go

type CommentCollection struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [AddThreadedComment_Int_Int_String_ThreadedCommentAuthor](./addthreadedcomment_int_int_string_threadedcommentauthor/) | Добавляет вложенный комментарий. |
| [AddThreadedComment_String_String_ThreadedCommentAuthor](./addthreadedcomment_string_string_threadedcommentauthor/) | Добавляет вложенный комментарий. |
| [GetThreadedComments_Int_Int](./getthreadedcomments_int_int/) | Получает вложенные комментарии по индексу строки и столбца. |
| [GetThreadedComments_String](./getthreadedcomments_string/) | Получает вложенные комментарии по имени ячейки. |
| [Add_Int_Int](./add_int_int/) | Добавляет комментарий в коллекцию. |
| [Add_String](./add_string/) | Добавляет комментарий в коллекцию. |
| [Get_Int](./get_int/) | Получает элемент Comment по указанному индексу. |
| [Get_String](./get_string/) | Получает элемент Comment по указанной ячейке. |
| [Get_Int_Int](./get_int_int/) | Получает элемент Comment по указанному индексу строки и индексу столбца. |
| [RemoveAt_String](./removeat_string/) | Удаляет комментарий конкретной ячейки. |
| [RemoveAt_Int_Int](./removeat_int_int/) | Удаляет комментарий конкретной ячейки. |
| [Clear](./clear/) | Удаляет все комментарии; |
| [GetCount](./getcount/) | Получает количество элементов, содержащихся в экземпляре. |
