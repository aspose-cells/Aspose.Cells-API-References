---
title: "Workbook.CreateCellsColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Crea un objeto CellsColor"
type: docs
url: /es/net/aspose.cells/workbook/createcellscolor/
---
## Workbook.CreateCellsColor method

Crea un objeto [`CellsColor`](../../cellscolor/)

```csharp
public CellsColor CreateCellsColor()
```

### Valor de retorno

Devuelve un objeto [`CellsColor`](../../cellscolor/)

### Ejemplos

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
            
            // Crear un rango y establecer bordes con color personalizado
            Aspose.Cells.Range range = workbook.Worksheets[0].Cells.CreateRange("B5:F10");
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            range.SetInsideBorders(BorderType.Horizontal, CellBorderType.Thin, color);

            // Verificar el estilo del borde en una celda específica
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

### Ver también

* class [CellsColor](../../cellscolor/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


