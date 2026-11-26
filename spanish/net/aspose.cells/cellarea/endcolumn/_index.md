---
title: "CellArea.EndColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Campo CellArea. Obtiene o establece la columna final de esta área"
type: docs
url: /es/net/aspose.cells/cellarea/endcolumn/
---
## CellArea.EndColumn field

Obtiene o establece la columna final de esta área.

```csharp
public int EndColumn;
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellAreaFieldEndColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crear un área de celdas desde A1 hasta C3
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 2;

            // Procesar el área de celdas usando EndColumn
            ProcessCellArea(area, Color.LightBlue, sheet);

            // Guarda el libro de trabajo
            workbook.Save("CellAreaFieldEndColumnDemo_output.xlsx");
        }

        private static void ProcessCellArea(CellArea area, Color color, Worksheet sheet)
        {
            int k = 0;
            for (int col = area.StartColumn; col <= area.EndColumn; col++)
            {
                for (int row = area.StartRow; row <= area.EndRow; row++)
                {
                    Cell cell = sheet.Cells[row, col];
                    
                    if (!color.IsEmpty)
                    {
                        Style style = cell.GetStyle();
                        style.ForegroundColor = color;
                        style.Pattern = BackgroundType.Solid;
                        cell.SetStyle(style);
                    }
                    
                    cell.PutValue(row + col + k);
                    k++;
                }
            }
        }
    }
}
```

### Ver también

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


