---
title: "Border.Color"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Border. Ottiene o imposta il colore del bordo"
type: docs
url: /it/net/aspose.cells/border/color/
---
## Border.Color property

Ottiene o imposta il colore del bordo.

```csharp
public Color Color { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla cella A1
            Cell cell = worksheet.Cells["A1"];
            
            // Imposta il valore della cella
            cell.PutValue("Border Color Demo");
            
            // Ottieni lo stile della cella
            Style style = cell.GetStyle();
            
            // Imposta i colori e gli stili del bordo
            style.Borders[BorderType.TopBorder].Color = Color.Red;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            
            style.Borders[BorderType.BottomBorder].Color = Color.Blue;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dotted;
            
            style.Borders[BorderType.LeftBorder].Color = Color.Green;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dashed;
            
            style.Borders[BorderType.RightBorder].Color = Color.FromArgb(255, 128, 0); // Orange
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            
            // Applica lo stile alla cella
            cell.SetStyle(style);
            
            // Salva la cartella di lavoro
            workbook.Save("BorderColorDemo.xlsx");
            
            Console.WriteLine("Border color demo created successfully.");
        }
    }
}
```

### Vedi anche

* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


