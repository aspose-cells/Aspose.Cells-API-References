---
title: "CellsColor.Argb"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CellsColor. Ottiene e imposta il colore da un valore ARGB a 32 bit"
type: docs
url: /it/net/aspose.cells/cellscolor/argb/
---
## CellsColor.Argb property

Ottiene e imposta il colore da un valore ARGB a 32 bit.

```csharp
public int Argb { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsColorPropertyArgbDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un intervallo e uno stile
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "A5");
            Style style = workbook.CreateStyle();

            // Crea e configura CellsColor usando la proprietà Argb
            CellsColor cellsColor = workbook.CreateCellsColor();
            cellsColor.Argb = Color.FromArgb(128, 0, 0, 255).ToArgb(); // Semi-transparent blue

            // Applica il colore allo stile
            style.ForegroundColor = cellsColor.Color;
            style.Pattern = BackgroundType.Solid;
            
            // Applica lo stile all'intervallo
            range.ApplyStyle(style, new StyleFlag { CellShading = true });

            // Salva la cartella di lavoro
            workbook.Save("CellsColorArgbDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


