---
title: "Style.Borders"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Ottiene la BorderCollection dello stile"
type: docs
url: /it/net/aspose.cells/style/borders/
---
## Style.Borders property

Ottiene la [`BorderCollection`](../../bordercollection/) dello stile.

```csharp
public BorderCollection Borders { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyBordersDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ottieni la cella e il suo stile
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            
            // Imposta diversi stili di bordo
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Medium;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thick;
            
            // Applica lo stile alla cella
            cell.SetStyle(style);
            
            // Salva la cartella di lavoro
            workbook.Save("BorderStylesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [BorderCollection](../../bordercollection/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


