---
title: "Range-Klasse"
linktitle: "Range"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "Range-Klasse. Kapselt das Objekt, das range in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/range/
---

## Range class

Kapselt das Objekt, das einen Zellbereich innerhalb einer Tabellenkalkulation darstellt.

```go

type Range struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewRange_CellArea_Cells](./newrange_cellarea_cells/) | Klassenkonstruktor. |
| [NewRange_Int_Int_Int_Int_Cells](./newrange_int_int_int_int_cells/) | Klassenkonstruktor. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [AutoFill_Range](./autofill_range/) | Füllt den Zielbereich automatisch aus. |
| [AutoFill_Range_AutoFillType](./autofill_range_autofilltype/) | Füllt den Zielbereich automatisch aus. |
| [GetCurrentRegion](./getcurrentregion/) | Gibt ein Range-Objekt zurück, das die aktuelle Region darstellt. Die aktuelle Region ist ein Bereich, der durch eine beliebige Kombination aus leeren Zeilen und leeren Spalten begrenzt wird. |
| [GetHyperlinks](./gethyperlinks/) | Ermittelt alle Hyperlinks im Bereich. |
| [AddHyperlink](./addhyperlink/) | Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu. |
| [GetEnumerator](./getenumerator/) | Ermittelt den Enumerator für Zellen in diesem Range. |
| [IsIntersect](./isintersect/) | Gibt an, ob der Bereich sich überschneidet. |
| [Intersect](./intersect/) | Gibt ein Range-Objekt zurück, das die rechteckige Schnittmenge zweier Bereiche darstellt. |
| [UnionRanges](./unionranges/) | Gibt das Ergebnis der Vereinigung zweier Bereiche zurück. |
| [GetRowCount](./getrowcount/) | Ermittelt die Anzahl der Zeilen im Bereich. |
| [GetColumnCount](./getcolumncount/) | Ermittelt die Anzahl der Spalten im Bereich. |
| [GetName](./getname/) | Liest oder legt den Namen des Bereichs fest. |
| [SetName](./setname/) | Liest oder legt den Namen des Bereichs fest. |
| [GetRefersTo](./getrefersto/) | Liest, worauf sich der Bereich bezieht. |
| [GetAddress](./getaddress/) | Liest die Adresse des Bereichs. |
| [IsBlank](./isblank/) | Gibt an, ob der Bereich Werte enthält. |
| [GetLeft](./getleft/) | Liest den Abstand in Punkten von der linken Kante von Spalte A bis zur linken Kante des Bereichs. |
| [GetTop](./gettop/) | Liest den Abstand in Punkten von der oberen Kante von Zeile 1 bis zur oberen Kante des Bereichs. |
| [GetWidth](./getwidth/) | Liest die Breite eines Bereichs in Punkten. |
| [GetHeight](./getheight/) | Liest die Breite eines Bereichs in Punkten. |
| [GetFirstRow](./getfirstrow/) | Liest den Index der ersten Zeile des Bereichs. |
| [GetFirstColumn](./getfirstcolumn/) | Liest den Index der ersten Spalte des Bereichs. |
| [Merge](./merge/) | Kombiniert einen Zellbereich zu einer einzelnen Zelle. |
| [UnMerge](./unmerge/) | Löst zusammengeführte Zellen dieses Bereichs. |
| [PutValue](./putvalue/) | Setzt einen Wert in den Bereich; falls erforderlich wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zelle zurückgesetzt. |
| [GetValue](./getvalue/) | Liest und legt den Wert des Bereichs fest. |
| [SetValue](./setvalue/) | Liest und legt den Wert des Bereichs fest. |
| [SetStyle_Style_Bool](./setstyle_style_bool/) | Wendet den Zellenstil an. |
| [ApplyStyle](./applystyle/) | Wendet Formate für einen gesamten Bereich an. |
| [SetStyle_Style](./setstyle_style/) | Legt den Stil des Bereichs fest. |
| [SetOutlineBorders_CellBorderType_CellsColor](./setoutlineborders_cellbordertype_cellscolor/) | Setzt die Umrandungsrahmen um einen Zellbereich mit demselben Rahmenstil und derselben Farbe. |
| [SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | Setzt die Umrandungsrahmen um einen Zellbereich mit demselben Rahmenstil und derselben Farbe. |
| [SetOutlineBorders_CellBorderTypeArray_ColorArray](./setoutlineborders_cellbordertypearray_colorarray/) | Setzt Umrandungsrahmen um einen Zellbereich. |
| [SetOutlineBorder_BorderType_CellBorderType_CellsColor](./setoutlineborder_bordertype_cellbordertype_cellscolor/) | Setzt den Umrandungsrahmen um einen Zellbereich. |
| [SetOutlineBorder_BorderType_CellBorderType_Color](./setoutlineborder_bordertype_cellbordertype_color/) | Setzt den Umrandungsrahmen um einen Zellbereich. |
| [SetInsideBorders](./setinsideborders/) | Setzt die inneren Rahmen des Bereichs. |
| [GetColumnWidth](./getcolumnwidth/) | Legt die Spaltenbreite dieses Bereichs fest oder liest sie |
| [SetColumnWidth](./setcolumnwidth/) | Legt die Spaltenbreite dieses Bereichs fest oder liest sie |
| [GetRowHeight](./getrowheight/) | Legt die Höhe der Zeilen in diesem Bereich fest oder liest sie |
| [SetRowHeight](./setrowheight/) | Legt die Höhe der Zeilen in diesem Bereich fest oder liest sie |
| [MoveTo](./moveto/) | Verschiebt den aktuellen Bereich zum Zielbereich. |
| [CopyData](./copydata/) | Kopiert Zellen­daten (einschließlich Formeln) aus einem Quellbereich. |
| [CopyValue](./copyvalue/) | Kopiert den Zellenwert aus einem Quellbereich. |
| [CopyStyle](./copystyle/) | Kopiert Stileinstellungen aus einem Quellbereich. |
| [Copy_Range_PasteOptions](./copy_range_pasteoptions/) | Kopieren des Bereichs mit Spezial‑Einfügeoptionen. |
| [Transpose](./transpose/) | Transponiert (dreht) Daten von Zeilen zu Spalten oder umgekehrt. |
| [Copy_Range](./copy_range/) | Kopiert Daten (einschließlich Formeln), Formatierungen, Zeichenobjekte usw. aus einem Quellbereich. |
| [Get](./get/) | Liefert das Cell‑Objekt in diesem Bereich. |
| [GetCellOrNull](./getcellornull/) | Liefert das Cell‑Objekt oder null in diesem Bereich. |
| [GetOffset](./getoffset/) | Liefert den Range‑Bereich nach Versatz. |
| [GetEntireColumn](./getentirecolumn/) | Liefert ein Range‑Objekt, das die gesamte Spalte (oder Spalten) repräsentiert, die den angegebenen Bereich enthält. |
| [GetEntireRow](./getentirerow/) | Liefert ein Range‑Objekt, das die gesamte Zeile (oder Zeilen) repräsentiert, die den angegebenen Bereich enthält. |
| [GetWorksheet](./getworksheet/) | Liefert das Worksheet‑Objekt, das diesen Bereich enthält. |
| [ToString](./tostring/) | Gibt einen String zurück, der das aktuelle Range‑Objekt darstellt. |
| [ToImage](./toimage/) | Konvertiert den Bereich in ein Bild. |
| [ToJson](./tojson/) | Konvertiert den Bereich in einen JSON‑Wert. |
| [ToHtml](./tohtml/) | Konvertiert den Bereich in HTML. |
| [Clear](./clear/) | Löscht diesen Bereich. |
| [ClearContents](./clearcontents/) | Löscht den Inhalt dieses Bereichs. |
| [ClearFormats](./clearformats/) | Löscht die Formate dieses Bereichs. |
| [ClearComments](./clearcomments/) | Löscht die Kommentare dieses Bereichs. |
| [ClearHyperlinks](./clearhyperlinks/) | Entfernt nur Hyperlinks. |
