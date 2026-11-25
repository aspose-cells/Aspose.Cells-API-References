---
title: "Workbook.CreateCellsColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Crea un oggetto CellsColor"
type: docs
url: /it/net/aspose.cells/workbook/createcellscolor/
---
## Workbook.CreateCellsColor method

Crea un oggetto [`CellsColor`](../../cellscolor/).

```csharp
public CellsColor CreateCellsColor()
```

### Valore di ritorno

Restituisce un oggetto [`CellsColor`](../../cellscolor/).

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateCellsColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Crea un intervallo e imposta i bordi con un colore personalizzato
            Aspose.Cells.Range range = workbook.Worksheets[0].Cells.CreateRange("B5:F10");
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            range.SetInsideBorders(BorderType.Horizontal, CellBorderType.Thin, color);

            // Verifica lo stile del bordo in una cella specifica
            Cell cell = workbook.Worksheets[0].Cells["F5"];
            Style style = cell.GetStyle();
            Console.WriteLine("Left Border: " + style.Borders[BorderType.LeftBorder].LineStyle);
            Console.WriteLine("Bottom Border: " + style.Borders[BorderType.BottomBorder].LineStyle);
            Console.WriteLine("Top Border: " + style.Borders[BorderType.TopBorder].LineStyle);
            Console.WriteLine("Right Border: " + style.Borders[BorderType.RightBorder].LineStyle);

            workbook.Save("CreateCellsColorExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [CellsColor](../../cellscolor/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


