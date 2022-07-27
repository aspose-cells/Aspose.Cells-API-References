---
title: Range
second_title: Aspose.Cells für .NET-API-Referenz
description: Kapselt das Objekt das einen Zellbereich innerhalb einer Tabelle darstellt.
type: docs
weight: 5030
url: /de/net/aspose.cells/range/
---
## Range class

Kapselt das Objekt, das einen Zellbereich innerhalb einer Tabelle darstellt.

```csharp
public class Range
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Address](../../aspose.cells/range/address) { get; } | Ruft die Adresse des Bereichs ab. |
| [ColumnCount](../../aspose.cells/range/columncount) { get; } | Ruft die Anzahl der Spalten im Bereich ab. |
| [ColumnWidth](../../aspose.cells/range/columnwidth) { get; set; } | Setzt oder erhält die Spaltenbreite dieses Bereichs |
| [CurrentRegion](../../aspose.cells/range/currentregion) { get; } | Gibt ein Range-Objekt zurück, das die aktuelle Region darstellt. Die aktuelle Region ist ein Bereich, der durch eine beliebige Kombination aus leeren Zeilen und leeren Spalten begrenzt ist. |
| [EntireColumn](../../aspose.cells/range/entirecolumn) { get; } | Ruft ein Range-Objekt ab, das die gesamte Spalte (oder Spalten) darstellt, die den angegebenen Bereich enthält. |
| [EntireRow](../../aspose.cells/range/entirerow) { get; } | Ruft ein Range-Objekt ab, das die gesamte Zeile (oder Zeilen) darstellt, die den angegebenen Bereich enthält. |
| [FirstColumn](../../aspose.cells/range/firstcolumn) { get; } | Ruft den Index der ersten Spalte des Bereichs ab. |
| [FirstRow](../../aspose.cells/range/firstrow) { get; } | Ruft den Index der ersten Zeile des Bereichs ab. |
| [Height](../../aspose.cells/range/height) { get; } | Ruft die Breite eines Bereichs in Punkten ab. |
| [Hyperlinks](../../aspose.cells/range/hyperlinks) { get; } | Ruft alle Hyperlinks im Bereich ab. |
| [Item](../../aspose.cells/range/item) { get; } | erhält[`Cell`](../cell) Objekt in diesem Bereich. |
| [Left](../../aspose.cells/range/left) { get; } | Ruft den Abstand in Punkt vom linken Rand der Spalte A zum linken Rand des Bereichs ab. |
| [Name](../../aspose.cells/range/name) { get; set; } | Ruft den Namen des Bereichs ab oder legt ihn fest. |
| [RefersTo](../../aspose.cells/range/refersto) { get; } | Ruft die Verweise des Bereichs ab. |
| [RowCount](../../aspose.cells/range/rowcount) { get; } | Ruft die Anzahl der Zeilen im Bereich ab. |
| [RowHeight](../../aspose.cells/range/rowheight) { get; set; } | Legt die Zeilenhöhe in diesem Bereich fest oder ruft sie ab |
| [Top](../../aspose.cells/range/top) { get; } | Ruft den Abstand in Punkt vom oberen Rand von Zeile 1 zum oberen Rand des Bereichs ab. |
| [Value](../../aspose.cells/range/value) { get; set; } | Ruft den Wert des Bereichs ab und legt ihn fest. |
| [Width](../../aspose.cells/range/width) { get; } | Ruft die Breite eines Bereichs in Punkten ab. |
| [Worksheet](../../aspose.cells/range/worksheet) { get; } | Ruft die ab[`Worksheet`](./worksheet) Objekt, das diesen Bereich enthält. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [ApplyStyle](../../aspose.cells/range/applystyle)(Style, StyleFlag) | Wendet Formate für einen ganzen Bereich an. |
| [AutoFill](../../aspose.cells/range/autofill#autofill)(Range) | Automatisches Füllen des Zielbereichs. |
| [AutoFill](../../aspose.cells/range/autofill#autofill_1)(Range, AutoFillType) | Automatisches Füllen des Zielbereichs. |
| [Copy](../../aspose.cells/range/copy#copy)(Range) | Kopiert Daten (einschließlich Formeln), Formatierungen, Zeichenobjekte usw. aus einem Quellbereich. |
| [Copy](../../aspose.cells/range/copy#copy_1)(Range, PasteOptions) | Kopieren des Bereichs mit Einfügen spezieller Optionen. |
| [CopyData](../../aspose.cells/range/copydata)(Range) | Kopiert Zelldaten (einschließlich Formeln) aus einem Quellbereich. |
| [CopyStyle](../../aspose.cells/range/copystyle)(Range) | Kopiert Stileinstellungen aus einem Quellbereich. |
| [CopyValue](../../aspose.cells/range/copyvalue)(Range) | Kopiert Zellenwert aus einem Quellbereich. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable#exportdatatable)() | Exportiert Daten in diesem Bereich nach aDataTable Objekt. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable#exportdatatable_1)(ExportTableOptions) | Exportiert Daten in diesem Bereich nach aDataTable Objekt. |
| [ExportDataTableAsString](../../aspose.cells/range/exportdatatableasstring)() | Exportiert Daten in diesem Bereich nach aDataTable Objekt. |
| [GetCellOrNull](../../aspose.cells/range/getcellornull)(int, int) | erhält[`Cell`](../cell) Objekt oder null in diesem Bereich. |
| [GetEnumerator](../../aspose.cells/range/getenumerator)() | Ruft den Enumerator für Zellen in diesem Bereich ab. |
| [GetOffset](../../aspose.cells/range/getoffset)(int, int) | erhält[`Range`](../range) Bereich durch Offset. |
| [Intersect](../../aspose.cells/range/intersect)(Range) | Gibt a zurück[`Range`](../range) Objekt, das den rechteckigen Schnittpunkt zweier Bereiche darstellt. |
| [IsIntersect](../../aspose.cells/range/isintersect)(Range) | Gibt an, ob sich der Bereich überschneidet. |
| [Merge](../../aspose.cells/range/merge)() | Kombiniert eine Reihe von Zellen zu einer einzigen Zelle. |
| [MoveTo](../../aspose.cells/range/moveto)(int, int) | Verschiebt den aktuellen Bereich in den Zielbereich. |
| [PutValue](../../aspose.cells/range/putvalue)(string, bool, bool) | Fügt einen Wert in den Bereich ein, gegebenenfalls wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zelle wird zurückgesetzt. |
| [SetInsideBorders](../../aspose.cells/range/setinsideborders)(BorderType, CellBorderType, CellsColor) | Innerhalb der Grenzen des Bereichs setzen. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder)(BorderType, CellBorderType, Color) | Legt den Umrissrahmen um einen Bereich von Zellen fest. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders#setoutlineborders)(CellBorderType, Color) | Legt die Umrisslinien um einen Bereich von Zellen mit demselben Rahmenstil und derselben Farbe fest. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders#setoutlineborders_1)(CellBorderType[], Color[]) | Legt Linienränder um einen Bereich von Zellen fest. |
| [SetStyle](../../aspose.cells/range/setstyle)(Style) | Legt den Stil des Bereichs fest. |
| override [ToString](../../aspose.cells/range/tostring)() | Gibt eine Zeichenfolge zurück, die das aktuelle Range-Objekt darstellt. |
| [Union](../../aspose.cells/range/union)(Range) | Gibt die Vereinigung zweier Bereiche zurück. |
| [UnMerge](../../aspose.cells/range/unmerge)() | Hebt verbundene Zellen dieses Bereichs auf. |

### Beispiele

```csharp

[C#]

//Instanziieren eines Workbook-Objekts
Workbook workbook = new Workbook();
// Holen Sie sich die ersten Arbeitsblattzellen.
Cells cells = workbook.Worksheets[0].Cells;
// Erstellen Sie einen Bereich (A1:D3).
Range range = cells.CreateRange("A1", "D3");
// Wert auf den Bereich setzen.
range.Value = "Hello";
//Excel-Datei speichern
workbook.Save("book1.xlsm");

 [Visual Basic]

'Instanziieren eines Workbook-Objekts
Dim workbook As Workbook = New Workbook()
'Holen Sie sich die ersten Arbeitsblattzellen.
Dim cells as Cells = workbook.Worksheets[0].Cells
'Erstellen Sie einen Bereich (A1:D3).
Dim range as Range = cells.CreateRange("A1", "D3")
'Stellen Sie den Wert auf den Bereich ein.
range.Value = "Hello"
'Speichern Sie die Excel-Datei
workbook.Save("book1.xlsm")
```

### Siehe auch

* namensraum [Aspose.Cells](../../aspose.cells)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
