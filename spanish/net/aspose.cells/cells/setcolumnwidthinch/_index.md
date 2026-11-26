---
title: "Cells.SetColumnWidthInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Establece el ancho de columna en unidades de pulgadas en vista normal"
type: docs
url: /es/net/aspose.cells/cells/setcolumnwidthinch/
---
## Cells.SetColumnWidthInch method

Establece el ancho de la columna en unidades de pulgadas en vista normal.

```csharp
public void SetColumnWidthInch(int column, double inches)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | Int32 | Índice de columna. |
| pulgadas | Double | Número de pulgadas. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetColumnWidthInchWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establece anchos de columna en pulgadas
            cells.SetColumnWidthInch(0, 2.0);
            cells.SetColumnWidthInch(1, 1.5);
            cells.SetColumnWidthInch(2, 0.8);

            // Establece algunos datos en las celdas para que el archivo sea visible
            cells["A1"].PutValue("Column A (2 inches)");
            cells["B1"].PutValue("Column B (1.5 inches)");
            cells["C1"].PutValue("Column C (0.8 inches)");

            // Guarda el libro de trabajo
            workbook.Save("ColumnWidthsInInches.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


