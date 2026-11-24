---
title: "Klasse Range"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Range-Klasse. Kapselt das Objekt, das einen Zellbereich innerhalb einer Tabellenkalkulation darstellt"
type: docs
url: /de/net/aspose.cells/range/
---
## Range class

Kapselt das Objekt, das einen Zellbereich innerhalb einer Tabellenkalkulation darstellt.

```csharp
public class Range : IEnumerable
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [Range](range/#constructor)(CellArea, Cells) | Klassenkonstruktor. |
| [Range](range/#constructor_1)(int, int, int, int, Cells) | Klassenkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Address](../../aspose.cells/range/address/) { get; } | Liefert die Adresse des Bereichs. |
| [ColumnCount](../../aspose.cells/range/columncount/) { get; } | Liefert die Anzahl der Spalten im Bereich. |
| [ColumnWidth](../../aspose.cells/range/columnwidth/) { get; set; } | Setzt oder liefert die Spaltenbreite dieses Bereichs |
| [CurrentRegion](../../aspose.cells/range/currentregion/) { get; } | Gibt ein Range-Objekt zurück, das die aktuelle Region darstellt. Die aktuelle Region ist ein Bereich, der durch eine beliebige Kombination aus leeren Zeilen und leeren Spalten begrenzt ist. |
| [EntireColumn](../../aspose.cells/range/entirecolumn/) { get; } | Liefert ein Range-Objekt, das die gesamte Spalte (oder die gesamten Spalten) enthält, die den angegebenen Bereich umfassen. |
| [EntireRow](../../aspose.cells/range/entirerow/) { get; } | Liefert ein Range-Objekt, das die gesamte Zeile (oder die gesamten Zeilen) enthält, die den angegebenen Bereich umfassen. |
| [FirstColumn](../../aspose.cells/range/firstcolumn/) { get; } | Liefert den Index der ersten Spalte des Bereichs. |
| [FirstRow](../../aspose.cells/range/firstrow/) { get; } | Liefert den Index der ersten Zeile des Bereichs. |
| [Height](../../aspose.cells/range/height/) { get; } | Liefert die Breite eines Bereichs in Punkten. |
| [Hyperlinks](../../aspose.cells/range/hyperlinks/) { get; } | Liefert alle Hyperlinks im Bereich. |
| [Item](../../aspose.cells/range/item/) { get; } | Liefert das [`Cell`](../cell/)-Objekt in diesem Bereich. |
| [Left](../../aspose.cells/range/left/) { get; } | Liefert den Abstand in Punkten von der linken Kante der Spalte A zur linken Kante des Bereichs. |
| [Name](../../aspose.cells/range/name/) { get; set; } | Liefert oder setzt den Namen des Bereichs. |
| [RefersTo](../../aspose.cells/range/refersto/) { get; } | Liefert das 'refers to' des Bereichs. |
| [RowCount](../../aspose.cells/range/rowcount/) { get; } | Liefert die Anzahl der Zeilen im Bereich. |
| [RowHeight](../../aspose.cells/range/rowheight/) { get; set; } | Setzt oder liefert die Höhe der Zeilen in diesem Bereich |
| [Top](../../aspose.cells/range/top/) { get; } | Liefert den Abstand in Punkten von der oberen Kante der Zeile 1 zur oberen Kante des Bereichs. |
| [Value](../../aspose.cells/range/value/) { get; set; } | Liefert und setzt den Wert des Bereichs. |
| [Width](../../aspose.cells/range/width/) { get; } | Liefert die Breite eines Bereichs in Punkten. |
| [Worksheet](../../aspose.cells/range/worksheet/) { get; } | Liefert das [`Worksheet`](./worksheet/)-Objekt, das diesen Bereich enthält. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddHyperlink](../../aspose.cells/range/addhyperlink/)(string, string, string) | Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu. |
| [ApplyStyle](../../aspose.cells/range/applystyle/)(Style, StyleFlag) | Wendet Formate für einen gesamten Bereich an. |
| [AutoFill](../../aspose.cells/range/autofill/#autofill)(Range) | Füllt den Zielbereich automatisch aus. |
| [AutoFill](../../aspose.cells/range/autofill/#autofill_1)(Range, AutoFillType) | Füllt den Zielbereich automatisch aus. |
| [Clear](../../aspose.cells/range/clear/)() | Löscht diesen Bereich. |
| [ClearComments](../../aspose.cells/range/clearcomments/)() | Löscht die Kommentare dieses Bereichs. |
| [ClearContents](../../aspose.cells/range/clearcontents/)() | Löscht den Inhalt dieses Bereichs. |
| [ClearFormats](../../aspose.cells/range/clearformats/)() | Löscht die Formate dieses Bereichs. |
| [ClearHyperlinks](../../aspose.cells/range/clearhyperlinks/)(bool) | Entfernt nur Hyperlinks. |
| [Copy](../../aspose.cells/range/copy/#copy)(Range) | Kopiert Daten (einschließlich Formeln), Formatierungen, Zeichenobjekte usw. aus einem Quellbereich. |
| [Copy](../../aspose.cells/range/copy/#copy_1)(Range, PasteOptions) | Kopieren des Bereichs mit Spezial‑Einfügeoptionen. |
| [CopyData](../../aspose.cells/range/copydata/)(Range) | Kopiert Zellen­daten (einschließlich Formeln) aus einem Quellbereich. |
| [CopyStyle](../../aspose.cells/range/copystyle/)(Range) | Kopiert Stil­einstellungen aus einem Quellbereich. |
| [CopyValue](../../aspose.cells/range/copyvalue/)(Range) | Kopiert den Zellenwert aus einem Quellbereich. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable/#exportdatatable)() | Exportiert Daten dieses Bereichs in ein DataTable‑Objekt. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable/#exportdatatable_1)(ExportTableOptions) | Exportiert Daten dieses Bereichs in ein DataTable‑Objekt. |
| [ExportDataTableAsString](../../aspose.cells/range/exportdatatableasstring/)() | Exportiert Daten dieses Bereichs in ein DataTable‑Objekt. |
| [GetCellOrNull](../../aspose.cells/range/getcellornull/)(int, int) | Ruft das [`Cell`](../cell/)‑Objekt oder null in diesem Bereich ab. |
| [GetEnumerator](../../aspose.cells/range/getenumerator/)() | Ruft den Enumerator für Zellen in diesem Range ab. |
| [GetOffset](../../aspose.cells/range/getoffset/)(int, int) | Ruft den `Range`‑Bereich mittels Offset ab. |
| [Intersect](../../aspose.cells/range/intersect/)(Range) | Gibt ein `Range`‑Objekt zurück, das die rechteckige Schnittmenge zweier Bereiche darstellt. |
| [IsBlank](../../aspose.cells/range/isblank/)() | Gibt an, ob der Bereich Werte enthält. |
| [IsIntersect](../../aspose.cells/range/isintersect/)(Range) | Gibt an, ob der Bereich sich schneidet. |
| [Merge](../../aspose.cells/range/merge/)() | Kombiniert einen Zellenbereich zu einer einzelnen Zelle. |
| [MoveTo](../../aspose.cells/range/moveto/)(int, int) | Verschiebt den aktuellen Bereich zum Zielbereich. |
| [PutValue](../../aspose.cells/range/putvalue/)(string, bool, bool) | Setzt einen Wert in den Bereich; falls zutreffend wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zelle zurückgesetzt. |
| [SetInsideBorders](../../aspose.cells/range/setinsideborders/)(BorderType, CellBorderType, CellsColor) | Setzt innere Rahmen des Bereichs. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder/#setoutlineborder)(BorderType, CellBorderType, CellsColor) | Setzt den Umrissrahmen um einen Zellenbereich. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder/#setoutlineborder_1)(BorderType, CellBorderType, Color) | Setzt den Umrissrahmen um einen Zellenbereich. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders)(CellBorderType, CellsColor) | Setzt die Umrissrahmen um einen Zellenbereich mit demselben Rahmenstil und derselben Farbe. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders_1)(CellBorderType, Color) | Setzt die Umrissrahmen um einen Zellenbereich mit demselben Rahmenstil und derselben Farbe. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders_2)(CellBorderType[], Color[]) | Setzt äußere Rahmen um einen Zellenbereich. |
| [SetStyle](../../aspose.cells/range/setstyle/#setstyle)(Style) | Legt den Stil des Bereichs fest. |
| [SetStyle](../../aspose.cells/range/setstyle/#setstyle_1)(Style, bool) | Wendet den Zellenstil an. |
| [ToHtml](../../aspose.cells/range/tohtml/)(HtmlSaveOptions) | Konvertiert den Bereich zu HTML. |
| [ToImage](../../aspose.cells/range/toimage/)(ImageOrPrintOptions) | Konvertiert den Bereich in ein Bild. |
| [ToJson](../../aspose.cells/range/tojson/)(JsonSaveOptions) | Konvertiert den Bereich in einen JSON-Wert. |
| override [ToString](../../aspose.cells/range/tostring/)() | Gibt einen String zurück, der das aktuelle Range-Objekt darstellt. |
| [Transpose](../../aspose.cells/range/transpose/)() | Transponiert (dreht) Daten von Zeilen zu Spalten oder umgekehrt. |
| [Union](../../aspose.cells/range/union/)(Range) | (**Obsolete.**) Gibt die Vereinigung von zwei Bereichen zurück. |
| [UnionRang](../../aspose.cells/range/unionrang/)(Range) | (**Obsolete.**) Gibt das Ergebnis der Vereinigung von zwei Bereichen zurück. |
| [UnionRanges](../../aspose.cells/range/unionranges/)(Range[]) | Gibt das Ergebnis der Vereinigung von zwei Bereichen zurück. |
| [UnMerge](../../aspose.cells/range/unmerge/)() | Löst zusammengeführte Zellen dieses Bereichs. |

### Hinweise

Die Range-Klasse bezeichnet einen Bereich einer Excel-Tabelle. Damit können Sie den Bereich formatieren und Werte festlegen. Und Sie können auch einfach einen Excel‑Bereich kopieren.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1", "D3");
            range.Value = "Hello";
            workbook.Save("book1.xlsm");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


