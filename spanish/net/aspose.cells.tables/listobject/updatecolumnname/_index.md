---
title: "ListObject.UpdateColumnName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de ListObject. Actualiza el nombre de todas las columnas de la lista a las celdas de la tabla"
type: docs
url: /es/net/aspose.cells.tables/listobject/updatecolumnname/
---
## ListObject.UpdateColumnName method

Actualiza el nombre de todas las columnas de lista a las celdas en la tabla.

```csharp
public void UpdateColumnName()
```

### Observaciones

El valor de las celdas en la fila de encabezado de la tabla debe ser igual al nombre del ListColumn; Cell.PutValue no modifica automáticamente el nombre del ListColumn por rendimiento.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListObjectMethodUpdateColumnNameDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Crear un objeto tabla/lista
            var listObject = ws.ListObjects[ws.ListObjects.Add(3, 3, 6, 6, true)];
            
            // Poblar algunos datos en la tabla
            for (int r = 0; r < 3; r++)
            {
                for (int c = 0; c < 3; c++)
                {
                    if (c > 0)
                        ws.Cells[listObject.StartRow + r, listObject.StartColumn + c].PutValue(r + c);
                    else
                        ws.Cells[listObject.StartRow + r, listObject.StartColumn + c].PutValue("");
                }
            }

            // Actualizar los nombres de columnas (establecerá nombres predeterminados como Column1, Column2, etc.)
            listObject.UpdateColumnName();

            // Guarda el libro de trabajo
            wb.Save("output.xlsx");

            // Verificar que el nombre de la columna se haya actualizado
            Console.WriteLine("First column name: " + ws.Cells[listObject.StartRow, listObject.StartColumn].StringValue);
        }
    }
}
```

### Ver también

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


