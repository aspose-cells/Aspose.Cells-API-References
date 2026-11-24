---
title: "Border.Color"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Border-Eigenschaft. Ruft die Farbe des Rahmens ab oder legt sie fest"
type: docs
url: /de/net/aspose.cells/border/color/
---
## Border.Color property

Liest oder setzt die Farbe des Rands.

```csharp
public Color Color { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BorderPropertyColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Zugriff auf Zelle A1
            Cell cell = worksheet.Cells["A1"];
            
            // Setzen Sie den Zellenwert
            cell.PutValue("Border Color Demo");
            
            // Den Stil der Zelle abrufen
            Style style = cell.GetStyle();
            
            // Legen Sie Rahmenfarben und -stile fest
            style.Borders[BorderType.TopBorder].Color = Color.Red;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            
            style.Borders[BorderType.BottomBorder].Color = Color.Blue;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dotted;
            
            style.Borders[BorderType.LeftBorder].Color = Color.Green;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dashed;
            
            style.Borders[BorderType.RightBorder].Color = Color.FromArgb(255, 128, 0); // Orange
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            
            // Wenden Sie den Stil auf die Zelle an
            cell.SetStyle(style);
            
            // Speichere die Arbeitsmappe
            workbook.Save("BorderColorDemo.xlsx");
            
            Console.WriteLine("Border color demo created successfully.");
        }
    }
}
```

### Siehe auch

* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


