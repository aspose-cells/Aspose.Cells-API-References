---
title: "WorksheetCollection.CreateRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WorksheetCollection. Crea un objeto Range a partir de una dirección del rango"
type: docs
url: /es/net/aspose.cells/worksheetcollection/createrange/
---
## WorksheetCollection.CreateRange method

Crea un objeto [`Range`](../../range/) a partir de una dirección del rango.

```csharp
public Range CreateRange(string address, int sheetIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| address | String | La dirección del rango. |
| sheetIndex | Int32 | El índice de la hoja. |

### Valor de retorno

Un objeto [`Range`](../../range/)

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodCreateRangeWithStringInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar algunos datos de muestra
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 6; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i+1},{j+1}");
                }
            }

            // Crear rango usando dirección de cadena e índice de hoja
            Aspose.Cells.Range range = workbook.Worksheets.CreateRange("A1:F10", 0);

            // Demostrar el uso del rango
            Console.WriteLine($"Range has {range.RowCount} rows and {range.ColumnCount} columns");
            Console.WriteLine($"First cell value: {range[0, 0].StringValue}");
            Console.WriteLine($"Last cell value: {range[9, 5].StringValue}");
        }
    }
}
```

### Ver también

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


