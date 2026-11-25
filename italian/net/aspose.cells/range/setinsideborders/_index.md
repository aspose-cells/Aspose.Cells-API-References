---
title: "Range.SetInsideBorders"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Imposta i bordi interni dell'intervallo"
type: docs
url: /it/net/aspose.cells/range/setinsideborders/
---
## Range.SetInsideBorders method

Imposta i bordi interni dell'intervallo.

```csharp
public void SetInsideBorders(BorderType borderEdge, CellBorderType lineStyle, 
    CellsColor borderColor)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| borderEdge | BorderType | Tipo di bordo interno, può essere solo Verticale o Orizzontale. |
| lineStyle | CellBorderType | Lo stile del bordo. |
| borderColor | CellsColor | Il colore del bordo. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangeMethodSetInsideBordersWithBorderTypeCellBorderTypeCellsCDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un intervallo e imposta i bordi interni
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B5:F10");
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            range.SetInsideBorders(BorderType.Vertical, CellBorderType.Thin, color);

            // Verifica i bordi in una cella all'interno dell'intervallo
            Cell cell = worksheet.Cells["C6"];
            Style style = cell.GetStyle();
            Console.WriteLine("Left Border: " + style.Borders[BorderType.LeftBorder].LineStyle);
            Console.WriteLine("Right Border: " + style.Borders[BorderType.RightBorder].LineStyle);
            Console.WriteLine("Top Border: " + style.Borders[BorderType.TopBorder].LineStyle);
            Console.WriteLine("Bottom Border: " + style.Borders[BorderType.BottomBorder].LineStyle);

            workbook.Save("SetInsideBordersExample.xlsx");
        }
    }
}
```

### Vedi anche

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


