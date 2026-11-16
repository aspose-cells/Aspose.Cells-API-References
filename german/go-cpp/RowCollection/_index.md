---
title: "RowCollection Klasse"
linktitle: "RowCollection"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "RowCollection Klasse. Kapselt das Objekt, das rowcollection in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/rowcollection/
---

## RowCollection class

Sammelt die <see cref="Row"/>-Objekte, die die einzelnen Zeilen in einem Arbeitsblatt darstellen.

```go

type RowCollection struct  {
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
| [GetCount](./getcount/) | Liefert die Anzahl der Zeilen in dieser Sammlung. |
| [GetEnumerator](./getenumerator/) | Liefert einen Enumerator, der die Zeilen dieser Sammlung durchläuft. |
| [GetEnumerator_Bool_Bool](./getenumerator_bool_bool/) | Liefert einen Enumerator, der die Zeilen dieser Sammlung durchläuft. |
| [GetRowByIndex](./getrowbyindex/) | Liefert das Zeilenobjekt anhand der Position in der Liste. |
| [Get](./get/) | Liefert ein Row-Objekt anhand des angegebenen Zeilenindex. Das Row-Objekt des angegebenen Zeilenindex wird instanziiert, falls es vorher nicht existiert. |
| [Clear](./clear/) | Alle Zeilen und Zellen löschen. |
| [RemoveAt](./removeat/) | Entfernt das Zeilen-Element am angegebenen Index (Position) in dieser Sammlung. |
