---
title: "CommentCollection‑Klasse"
linktitle: "CommentCollection"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "CommentCollection‑Klasse. Kapselt das Objekt, das commentcollection in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/commentcollection/
---

## CommentCollection class

Kapselt eine Sammlung von <see cref=\"Comment\"/>‑Objekten.

```go

type CommentCollection struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [AddThreadedComment_Int_Int_String_ThreadedCommentAuthor](./addthreadedcomment_int_int_string_threadedcommentauthor/) | Fügt einen Threaded‑Kommentar hinzu. |
| [AddThreadedComment_String_String_ThreadedCommentAuthor](./addthreadedcomment_string_string_threadedcommentauthor/) | Fügt einen Threaded‑Kommentar hinzu. |
| [GetThreadedComments_Int_Int](./getthreadedcomments_int_int/) | Liefert die Threaded‑Kommentare nach Zeilen‑ und Spaltenindex. |
| [GetThreadedComments_String](./getthreadedcomments_string/) | Liefert die Threaded‑Kommentare nach Zellnamen. |
| [Add_Int_Int](./add_int_int/) | Fügt der Sammlung einen Kommentar hinzu. |
| [Add_String](./add_string/) | Fügt der Sammlung einen Kommentar hinzu. |
| [Get_Int](./get_int/) | Liefert das Comment‑Element am angegebenen Index. |
| [Get_String](./get_string/) | Liefert das Comment‑Element in der angegebenen Zelle. |
| [Get_Int_Int](./get_int_int/) | Liefert das Comment‑Element am angegebenen Zeilen‑ und Spaltenindex. |
| [RemoveAt_String](./removeat_string/) | Entfernt den Kommentar der angegebenen Zelle. |
| [RemoveAt_Int_Int](./removeat_int_int/) | Entfernt den Kommentar der angegebenen Zelle. |
| [Clear](./clear/) | Entfernt alle Kommentare; |
| [GetCount](./getcount/) | Liefert die Anzahl der im Objekt enthaltenen Elemente. |
