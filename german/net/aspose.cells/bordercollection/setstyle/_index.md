---
title: "BorderCollection.SetStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BorderCollection-Methode. Legt den Stil aller Ränder der Sammlung fest."
type: docs
url: /de/net/aspose.cells/bordercollection/setstyle/
---
## BorderCollection.SetStyle method

Setzt den Stil aller Rahmen der Sammlung.

```csharp
public void SetStyle(CellBorderType style)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stil | CellBorderType | Stil der Ränder |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderCollectionMethodSetStyleWithCellBorderTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hole Zelle C6 und ihren Stil.
            Cell cell = worksheet.Cells["C6"];
            Style style = cell.GetStyle();

            // Setze Randfarbe und Stil.
            style.Borders.SetColor(System.Drawing.Color.Red);
            style.Borders.SetStyle(CellBorderType.Thick);

            // Wenden Sie den Stil auf die Zelle an
            cell.SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("BorderCollectionMethodSetStyleWithCellBorderTypeDemo_out.xlsx");

            Console.WriteLine("Border style set successfully.");
        }
    }
}
```

### Siehe auch

* enum [CellBorderType](../../cellbordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


