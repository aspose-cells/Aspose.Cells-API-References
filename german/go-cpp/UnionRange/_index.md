---
title: "UnionRange-Klasse"
linktitle: "UnionRange"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "UnionRange-Klasse. Kapselt das Objekt, das unionrange in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/unionrange/
---

## UnionRange class

Stellt einen Union‑Bereich dar.

```go

type UnionRange struct  {
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
| [GetFirstRow](./getfirstrow/) | Liest den Index der ersten Zeile des Bereichs. |
| [GetFirstColumn](./getfirstcolumn/) | Liest den Index der ersten Spalte des Bereichs. |
| [GetRowCount](./getrowcount/) | Ermittelt die Anzahl der Zeilen im Bereich. |
| [GetColumnCount](./getcolumncount/) | Ermittelt die Anzahl der Zeilen im Bereich. |
| [Merge](./merge/) | Kombiniert einen Zellbereich zu einer einzelnen Zelle. |
| [UnMerge](./unmerge/) | Löst zusammengeführte Zellen dieses Bereichs. |
| [PutValue](./putvalue/) | Setzt einen Wert in den Bereich; falls erforderlich wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zelle zurückgesetzt. |
| [GetValue](./getvalue/) | Liest und setzt die Werte des Bereichs. |
| [SetValue](./setvalue/) | Liest und setzt die Werte des Bereichs. |
| [GetName](./getname/) | Liest oder legt den Namen des Bereichs fest. |
| [SetName](./setname/) | Liest oder legt den Namen des Bereichs fest. |
| [GetRefersTo](./getrefersto/) | Liest, worauf sich der Bereich bezieht. |
| [GetHasRange](./gethasrange/) | Gibt an, ob dies einen Bereich hat. |
| [GetHyperlinks](./gethyperlinks/) | Ermittelt alle Hyperlinks im Bereich. |
| [SetStyle](./setstyle/) | Legt den Stil des Bereichs fest. |
| [ApplyStyle](./applystyle/) | Wendet Formate für einen gesamten Bereich an. |
| [Copy](./copy/) | Kopieren des Bereichs mit Spezial‑Einfügeoptionen. |
| [GetEnumerator](./getenumerator/) | Ermittelt den Enumerator für Zellen in diesem Range. |
| [GetCellCount](./getcellcount/) | Liefert die Gesamtzahl der Zellen im Bereich. |
| [GetRangeCount](./getrangecount/) | Liefert die Anzahl der Bereiche. |
| [GetRanges](./getranges/) | Liefert alle Union-Bereiche. |
| [SetOutlineBorders_CellBorderTypeArray_ColorArray](./setoutlineborders_cellbordertypearray_colorarray/) | Setzt Umrandungsrahmen um einen Zellbereich. |
| [SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | Setzt die Umrandungsrahmen um einen Zellbereich mit demselben Rahmenstil und derselben Farbe. |
| [Intersect_String](./intersect_string/) | Schneidet einen anderen Bereich. |
| [Intersect_UnionRange](./intersect_unionrange/) | Schneidet einen anderen Bereich. |
| [Intersect_RangeArray](./intersect_rangearray/) | Schneidet einen anderen Bereich. |
| [Union_String](./union_string/) | Vereint einen anderen Bereich. |
| [Union_UnionRange](./union_unionrange/) | Vereint einen anderen Bereich. |
| [Union_RangeArray](./union_rangearray/) | Vereint die Bereiche. |
