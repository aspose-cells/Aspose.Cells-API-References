---
title: "PivotTable.GetSourceDataConnections"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotTable. Obtiene las fuentes de datos de conexión externa"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/getsourcedataconnections/
---
## PivotTable.GetSourceDataConnections method

Obtiene las fuentes de datos de conexión externa.

```csharp
public ExternalConnection[] GetSourceDataConnections()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetSourceDataConnectionsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            
            // Crear tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Obtener conexiones de datos de origen
            ExternalConnection[] connections = pivotTable.GetSourceDataConnections();
            
            // Muestra la información de la conexión
            if (connections.Length > 0)
            {
                ExternalConnection conn = connections[0];
                Console.WriteLine("Connection Name: " + conn.Name);
                Console.WriteLine("Class Type: " + conn.ClassType);
                Console.WriteLine("Source Type: " + conn.SourceType);
                Console.WriteLine("Command: " + conn.Command);
            }
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableSourceConnections.xlsx");
        }
    }
}
```

### Ver también

* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


