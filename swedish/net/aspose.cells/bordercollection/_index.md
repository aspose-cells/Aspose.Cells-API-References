---
title: "Klassen BorderCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.BorderCollection-klass. Inkapslar en samling av Border-objekt"
type: docs
url: /sv/net/aspose.cells/bordercollection/
---
## BorderCollection class

Inkapslar en samling av [`Border`](../border/) objekt.

```csharp
public class BorderCollection
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [DiagonalColor](../../aspose.cells/bordercollection/diagonalcolor/) { get; set; } | Hämtar eller anger Color för diagonala linjer. |
| [DiagonalStyle](../../aspose.cells/bordercollection/diagonalstyle/) { get; set; } | Hämtar eller anger style för diagonala linjer. |
| [IsOutline](../../aspose.cells/bordercollection/isoutline/) { get; set; } | Anger om vänster, höger, övre och nedre kanter ska tillämpas endast på yttre kanter av ett cellområde. Standardvärdet är true. |
| [Item](../../aspose.cells/bordercollection/item/) { get; } | Hämtar [`Border`](../border/) elementet på det angivna indexet. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [SetColor](../../aspose.cells/bordercollection/setcolor/)(Color) | Anger Color för alla kanter i samlingen. |
| [SetStyle](../../aspose.cells/bordercollection/setstyle/)(CellBorderType) | Anger style för alla kanter i samlingen. |

### Exempel

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
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();

            // Lägga till ett nytt kalkylblad i Workbook-objektet
            workbook.Worksheets.Add();

            // Hämtar referensen till det nyligen tillagda kalkylbladet genom att ange dess bladindex
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till cellen "A1" från kalkylbladet
            Cell cell = worksheet.Cells["A1"];

            // Lägger till ett värde i cellen "A1"
            cell.PutValue("Visit Aspose!");

            // Hämtar stil för cellen
            Style style = cell.GetStyle();

            // Anger linjestil för den övre kanten
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;

            // Anger färg för den övre kanten
            style.Borders[BorderType.TopBorder].Color = Color.Red;

            // Anger linjestil för den nedre kanten
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thick;

            // Anger färg för den nedre kanten
            style.Borders[BorderType.BottomBorder].Color = Color.Green;

            // Anger linjestil för den vänstra kanten
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dashed;

            // Anger färg för den vänstra kanten
            style.Borders[BorderType.LeftBorder].Color = Color.Yellow;

            // Anger linjestil för den högra kanten
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Dotted;

            // Anger färg för den högra kanten
            style.Borders[BorderType.RightBorder].Color = Color.Blue;

            // Anger diagonala egenskaper
            style.Borders.DiagonalColor = Color.Red;
            style.Borders.DiagonalStyle = CellBorderType.Dashed;

            // Tillämpar stilen på cellen
            cell.SetStyle(style);

            // Sparar Excel-filen
            workbook.Save("BorderCollectionExample.xlsx");
            workbook.Save("BorderCollectionExample.pdf");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


