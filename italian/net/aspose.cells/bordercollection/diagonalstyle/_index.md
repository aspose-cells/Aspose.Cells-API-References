---
title: "BorderCollection.DiagonalStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BorderCollection. Ottiene o imposta lo stile delle linee diagonali"
type: docs
url: /it/net/aspose.cells/bordercollection/diagonalstyle/
---
## BorderCollection.DiagonalStyle property

Ottiene o imposta lo stile delle linee diagonali.

```csharp
public CellBorderType DiagonalStyle { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BorderCollectionPropertyDiagonalStyleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ottieni una cella e il suo stile
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            
            // Imposta le proprietà del bordo diagonale
            style.Borders.DiagonalStyle = CellBorderType.Thin;
            style.Borders.DiagonalColor = Color.Red;
            
            // Applica lo stile alla cella
            cell.SetStyle(style);
            
            // Salva la cartella di lavoro
            workbook.Save("DiagonalBorderDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [CellBorderType](../../cellbordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


