---
title: "Klasse BorderCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.BorderCollection Klasse. Kapselt eine Sammlung von Border-Objekten"
type: docs
url: /de/net/aspose.cells/bordercollection/
---
## BorderCollection class

Kapselt eine Sammlung von [`Border`](../border/) Objekten.

```csharp
public class BorderCollection
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [DiagonalColor](../../aspose.cells/bordercollection/diagonalcolor/) { get; set; } | Liest oder setzt die Farbe der Diagonallinien. |
| [DiagonalStyle](../../aspose.cells/bordercollection/diagonalstyle/) { get; set; } | Liest oder setzt den Stil der Diagonallinien. |
| [IsOutline](../../aspose.cells/bordercollection/isoutline/) { get; set; } | Gibt an, ob linke, rechte, obere und untere Rahmen nur auf die äußeren Rahmen eines Zellenbereichs angewendet werden sollen. Der Standardwert ist true. |
| [Item](../../aspose.cells/bordercollection/item/) { get; } | Liest das [`Border`](../border/) Element am angegebenen Index. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetColor](../../aspose.cells/bordercollection/setcolor/)(Color) | Setzt die Farbe aller Rahmen in der Sammlung. |
| [SetStyle](../../aspose.cells/bordercollection/setstyle/)(CellBorderType) | Setzt den Stil aller Rahmen der Sammlung. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BorderCollectionDemo
    {
        public static void BorderCollectionExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();

            // Hinzufügen eines neuen Arbeitsblatts zum Workbook-Objekt
            workbook.Worksheets.Add();

            // Abrufen der Referenz des neu hinzugefügten Arbeitsblatts durch Übergabe seines Blattindexes
            Worksheet worksheet = workbook.Worksheets[0];

            // Zugriff auf die Zelle "A1" aus dem Arbeitsblatt
            Cell cell = worksheet.Cells["A1"];

            // Hinzufügen eines Werts zur Zelle "A1"
            cell.PutValue("Visit Aspose!");

            // Abrufen des Stils der Zelle
            Style style = cell.GetStyle();

            // Festlegen des Linienstils des oberen Rahmens
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;

            // Festlegen der Farbe des oberen Rahmens
            style.Borders[BorderType.TopBorder].Color = Color.Red;

            // Festlegen des Linienstils des unteren Rahmens
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thick;

            // Festlegen der Farbe des unteren Rahmens
            style.Borders[BorderType.BottomBorder].Color = Color.Green;

            // Festlegen des Linienstils des linken Rahmens
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dashed;

            // Festlegen der Farbe des linken Rahmens
            style.Borders[BorderType.LeftBorder].Color = Color.Yellow;

            // Festlegen des Linienstils des rechten Rahmens
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Dotted;

            // Festlegen der Farbe des rechten Rahmens
            style.Borders[BorderType.RightBorder].Color = Color.Blue;

            // Festlegen diagonaler Eigenschaften
            style.Borders.DiagonalColor = Color.Red;
            style.Borders.DiagonalStyle = CellBorderType.Dashed;

            // Den Stil auf die Zelle anwenden
            cell.SetStyle(style);

            // Die Excel-Datei speichern
            workbook.Save("BorderCollectionExample.xlsx");
            workbook.Save("BorderCollectionExample.pdf");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


