---
title: "BorderCollection.SetColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BorderCollection‑metod. Anger färgen på alla kanter i samlingen"
type: docs
url: /sv/net/aspose.cells/bordercollection/setcolor/
---
## BorderCollection.SetColor method

Anger Color för alla kanter i samlingen.

```csharp
public void SetColor(Color color)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| färg | Färg | Kantens färg. |

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderCollectionMethodSetColorWithColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en stil med färgade kanter
            Style style = workbook.CreateStyle();
            
            // Ange kantlinjestilar
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            // Ange kantfärgen till röd med SetColor‑metoden
            style.Borders.SetColor(Color.Red);

            // Tillämpa stilen på en cell
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Cell with colored borders");
            cell.SetStyle(style);

            // Autoanpassa kolumn för bättre synlighet
            worksheet.AutoFitColumn(0);

            // Spara arbetsboken
            workbook.Save("BorderColorDemo.xlsx");
        }
    }
}
```

### Se även

* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


