---
title: "ExternalConnection.ConnectionString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnection. La cadena de información de conexión se utiliza para contactar con una fuente de datos OLE DB u ODBC"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/connectionstring/
---
## ExternalConnection.ConnectionString property

La cadena de información de conexión se usa para contactar con una fuente de datos OLE DB o ODBC.

```csharp
public virtual string ConnectionString { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyConnectionStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear datos de ejemplo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1500);
            
            // Crear una tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Obtener las conexiones de datos
            ExternalConnection[] connections = pivotTable.GetSourceDataConnections();
            
            // Mostrar la cadena de conexión si existe
            if (connections.Length > 0)
            {
                Console.WriteLine("Connection String: " + connections[0].ConnectionString);
            }
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableWithConnection.xlsx");
        }
    }
}
```

### Ver también

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


