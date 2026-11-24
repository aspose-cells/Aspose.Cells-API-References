---
title: "Klasse UnionRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.UnionRange Klasse. Stellt einen Union-Bereich dar"
type: docs
url: /de/net/aspose.cells/unionrange/
---
## UnionRange class

Stellt einen Union‑Bereich dar.

```csharp
public class UnionRange : IEnumerable
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CellCount](../../aspose.cells/unionrange/cellcount/) { get; } | Ermittelt die gesamte Zellanzahl im Bereich. |
| [ColumnCount](../../aspose.cells/unionrange/columncount/) { get; } | Liefert die Anzahl der Zeilen im Bereich. |
| [FirstColumn](../../aspose.cells/unionrange/firstcolumn/) { get; } | Liefert den Index der ersten Spalte des Bereichs. |
| [FirstRow](../../aspose.cells/unionrange/firstrow/) { get; } | Liefert den Index der ersten Zeile des Bereichs. |
| [HasRange](../../aspose.cells/unionrange/hasrange/) { get; } | Gibt an, ob dies einen Bereich hat. |
| [Hyperlinks](../../aspose.cells/unionrange/hyperlinks/) { get; } | Liefert alle Hyperlinks im Bereich. |
| [Name](../../aspose.cells/unionrange/name/) { get; set; } | Liefert oder setzt den Namen des Bereichs. |
| [RangeCount](../../aspose.cells/unionrange/rangecount/) { get; } | Ermittelt die Anzahl der Bereiche. |
| [Ranges](../../aspose.cells/unionrange/ranges/) { get; } | Ermittelt alle Vereinigungsbereiche. |
| [RefersTo](../../aspose.cells/unionrange/refersto/) { get; } | Liefert das 'refers to' des Bereichs. |
| [RowCount](../../aspose.cells/unionrange/rowcount/) { get; } | Liefert die Anzahl der Zeilen im Bereich. |
| [Value](../../aspose.cells/unionrange/value/) { get; set; } | Liest und setzt die Werte des Bereichs. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [ApplyStyle](../../aspose.cells/unionrange/applystyle/)(Style, StyleFlag) | Wendet Formate für einen gesamten Bereich an. |
| [Copy](../../aspose.cells/unionrange/copy/)(UnionRange, PasteOptions) | Kopieren des Bereichs mit Spezial‑Einfügeoptionen. |
| [GetEnumerator](../../aspose.cells/unionrange/getenumerator/)() | Ruft den Enumerator für Zellen in diesem Range ab. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect)(Range[]) | Schneidet einen anderen Bereich. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect_2)(string) | Schneidet einen anderen Bereich. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect_1)(UnionRange) | Schneidet einen anderen Bereich. |
| [Merge](../../aspose.cells/unionrange/merge/)() | Kombiniert einen Zellenbereich zu einer einzelnen Zelle. |
| [PutValue](../../aspose.cells/unionrange/putvalue/)(string, bool, bool) | Setzt einen Wert in den Bereich; falls zutreffend wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zelle zurückgesetzt. |
| [SetOutlineBorders](../../aspose.cells/unionrange/setoutlineborders/#setoutlineborders)(CellBorderType, Color) | Setzt die Umrissrahmen um einen Zellenbereich mit demselben Rahmenstil und derselben Farbe. |
| [SetOutlineBorders](../../aspose.cells/unionrange/setoutlineborders/#setoutlineborders_1)(CellBorderType[], Color[]) | Setzt äußere Rahmen um einen Zellenbereich. |
| [SetStyle](../../aspose.cells/unionrange/setstyle/)(Style) | Legt den Stil des Bereichs fest. |
| [Union](../../aspose.cells/unionrange/union/#union)(Range[]) | Vereint die Bereiche. |
| [Union](../../aspose.cells/unionrange/union/#union_2)(string) | Vereint einen anderen Bereich. |
| [Union](../../aspose.cells/unionrange/union/#union_1)(UnionRange) | Vereint einen anderen Bereich. |
| [UnMerge](../../aspose.cells/unionrange/unmerge/)() | Löst zusammengeführte Zellen dieses Bereichs. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassUnionRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle einen Vereinigungsbereich mit der richtigen API
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A10,C1:C10", 0);
            
            // Setze den Wert für den gesamten Vereinigungsbereich
            unionRange.Value = "Test";
            
            // Wende Stil auf den Vereinigungsbereich an
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            unionRange.ApplyStyle(style, new StyleFlag { All = true });
            
            // Speichere die Arbeitsmappe
            workbook.Save("UnionRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


