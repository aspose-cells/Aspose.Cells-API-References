---
title: "RevisionCellComment Klasse"
linktitle: "RevisionCellComment"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "RevisionCellComment Klasse. Kapselt das Objekt, das revisioncellcomment in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/revisioncellcomment/
---

## RevisionCellComment class

Stellt einen Revisionsdatensatz einer Zellkommentaränderung dar.

```go

type RevisionCellComment struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewRevisionCellComment](./newrevisioncellcomment/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetType](./gettype/) | Liest den Typ der Revision. |
| [GetRow](./getrow/) | Ermittelt den Zeilenindex, der einen Kommentar enthält. |
| [GetColumn](./getcolumn/) | Ermittelt den Spaltenindex, der einen Kommentar enthält. |
| [GetCellName](./getcellname/) | Liefert den Namen der Zelle. |
| [SetCellName](./setcellname/) | Liefert den Namen der Zelle. |
| [GetActionType](./getactiontype/) | Ermittelt den Aktionstyp der Revision. |
| [IsOldComment](./isoldcomment/) | Gibt an, ob es ein alter Kommentar ist. |
| [GetOldLength](./getoldlength/) | Ermittelt die Länge des Kommentartexts, der in dieser Revision hinzugefügt wurde. |
| [GetNewLength](./getnewlength/) | Ermittelt die Länge des Kommentars, bevor diese Revision vorgenommen wurde. |
| [GetWorksheet](./getworksheet/) | Liefert das Arbeitsblatt. |
| [GetId](./getid/) | Liefert die Nummer dieser Revision. |
