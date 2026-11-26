---
title: "Cells.GetLastDataRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene el índice de la última fila de la celda que contiene datos en la columna especificada"
type: docs
url: /es/net/aspose.cells/cells/getlastdatarow/
---
## Cells.GetLastDataRow method

Obtiene el índice de la última fila de la celda que contiene datos en la columna especificada.

```csharp
public int GetLastDataRow(int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | Int32 | Índice de columna. |

### Valor de retorno

índice de la última fila.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetLastDataRowWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["A4"].PutValue("Data3");
            
            // Obtener la última fila de datos en la columna A (índice 0)
            int lastRow = worksheet.Cells.GetLastDataRow(0);
            
            // Mostrar el resultado
            Console.WriteLine("Last data row in column A: " + lastRow);
            
            // Insertar una nueva fila después de la última fila de datos
            CellArea area = new CellArea();
            area.StartRow = lastRow + 1;
            area.EndRow = lastRow + 1;
            area.StartColumn = 0;
            area.EndColumn = 0;
            worksheet.Cells.InsertRange(area, 1, ShiftType.Down);
            
            // Agregar datos a la nueva fila
            worksheet.Cells[lastRow + 2, 0].PutValue("New Data");
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


