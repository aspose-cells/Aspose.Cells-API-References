---
title: "Clase QueryTable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.QueryTable. Representa la información de QueryTable"
type: docs
url: /es/net/aspose.cells/querytable/
---
## QueryTable class

Representa la información de QueryTable.

```csharp
public class QueryTable
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AdjustColumnWidth](../../aspose.cells/querytable/adjustcolumnwidth/) { get; set; } | Devuelve o establece el AdjustColumnWidth del objeto. |
| [ConnectionId](../../aspose.cells/querytable/connectionid/) { get; } | Obtiene el id de conexión de la tabla de consulta. |
| [ExternalConnection](../../aspose.cells/querytable/externalconnection/) { get; } | Obtiene la conexión externa relacionada. |
| [Name](../../aspose.cells/querytable/name/) { get; } | Obtiene el nombre de la querytable. |
| [PreserveFormatting](../../aspose.cells/querytable/preserveformatting/) { get; set; } | Devuelve o establece el PreserveFormatting del objeto. |
| [ResultRange](../../aspose.cells/querytable/resultrange/) { get; } | Obtiene el rango del resultado. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassQueryTableDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregue datos de muestra para crear una tabla de consulta (simulando datos externos)
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");
            
            // Verifique si hay tablas de consulta en la hoja de cálculo
            if (worksheet.QueryTables.Count > 0)
            {
                // Obtenga la primera tabla de consulta
                QueryTable qt = worksheet.QueryTables[0];
                
                // Mostrar propiedades de la tabla de consulta
                Console.WriteLine("Query Table Name: " + qt.Name);
                Console.WriteLine("Connection ID: " + qt.ConnectionId);
                Console.WriteLine("Result Range: " + qt.ResultRange.Address);
                Console.WriteLine("Preserve Formatting: " + qt.PreserveFormatting);
                Console.WriteLine("Adjust Column Width: " + qt.AdjustColumnWidth);
                
                // Modificar algunas propiedades
                qt.PreserveFormatting = true;
                qt.AdjustColumnWidth = false;
            }
            else
            {
                Console.WriteLine("No query tables found in the worksheet.");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


