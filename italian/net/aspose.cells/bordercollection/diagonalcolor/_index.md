---
title: "BorderCollection.DiagonalColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BorderCollection. Ottiene o imposta il colore delle linee diagonali"
type: docs
url: /it/net/aspose.cells/bordercollection/diagonalcolor/
---
## BorderCollection.DiagonalColor property

Ottiene o imposta il Color delle linee diagonali.

```csharp
public Color DiagonalColor { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BorderCollectionPropertyDiagonalColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Diagonal Border Demo");

            Style style = cell.GetStyle();
            
            // Impostazione delle proprietà del bordo diagonale
            style.Borders.DiagonalColor = Color.Red;
            style.Borders.DiagonalStyle = CellBorderType.Thick;

            cell.SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("DiagonalBorderDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


