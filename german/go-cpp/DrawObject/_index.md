---
title: "DrawObject Klasse"
linktitle: "DrawObject"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "DrawObject Klasse. Kapselt das Objekt, das drawobject in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/drawobject/
---

## DrawObject class

DrawObject wird beim Rendern initialisiert und zurückgegeben.

```go

type DrawObject struct  {
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
| [GetCell](./getcell/) | Gibt das Cell-Objekt beim Rendern an. Alle Eigenschaften der Zelle können zugegriffen werden. |
| [GetShape](./getshape/) | Gibt das Shape-Objekt beim Rendern an. Alle Eigenschaften von shape können zugegriffen werden. |
| [GetImageBytes](./getimagebytes/) | Gibt die Bildbytes des gerenderten Chart, Shape beim Rendern an. |
| [GetType](./gettype/) | Gibt den Typ von DrawObject an. |
| [GetCurrentPage](./getcurrentpage/) | Gibt den Seitenindex von DrawObject an. Der Seitenindex beginnt bei Null. Ein Blatt enthält mehrere Seiten beim Rendern. |
| [GetTotalPages](./gettotalpages/) | Gibt die Gesamtseitenzahl im aktuellen Rendering an. |
| [GetSheetIndex](./getsheetindex/) | Gibt den aktuellen Blattindex von DrawObject an. |
