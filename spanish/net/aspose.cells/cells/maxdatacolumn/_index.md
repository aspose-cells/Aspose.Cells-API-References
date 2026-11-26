---
title: "Cells.MaxDataColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Índice máximo de columna de la celda que contiene datos"
type: docs
url: /es/net/aspose.cells/cells/maxdatacolumn/
---
## Cells.MaxDataColumn property

Índice máximo de columna de la celda que contiene datos.

```csharp
public int MaxDataColumn { get; }
```

### Observaciones

-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Data;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxDataColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(300);
            worksheet.Cells["B3"].PutValue(400);

            // Obtenga el índice máximo de columna de datos (basado en 0)
            int maxColumn = worksheet.Cells.MaxDataColumn;
            Console.WriteLine("Max Data Column: " + maxColumn);

            // Exporte datos usando MaxDataColumn
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 
                worksheet.Cells.MaxDataRow + 1, 
                worksheet.Cells.MaxDataColumn + 1);

            // Muestre los datos exportados
            Console.WriteLine("Exported Data:");
            foreach (DataRow row in dataTable.Rows)
            {
                for (int i = 0; i <= maxColumn; i++)
                {
                    Console.Write(row[i] + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


