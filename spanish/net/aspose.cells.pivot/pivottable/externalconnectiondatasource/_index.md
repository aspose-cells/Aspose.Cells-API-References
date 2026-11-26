---
title: "PivotTable.ExternalConnectionDataSource"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Obtiene la fuente de datos de conexión externa"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/externalconnectiondatasource/
---
## PivotTable.ExternalConnectionDataSource property

Obtiene la fuente de datos de conexión externa.

```csharp
[Obsolete("Use PivotTable.GetSourceDataConnections() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ExternalConnection ExternalConnectionDataSource { get; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice el método PivotTable.GetSourceDataConnections(). Este método será eliminado 12 meses después a partir de octubre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyExternalConnectionDataSourceDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con conexión de datos externa
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Crear datos de ejemplo
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["B3"].PutValue(2000);

            // Agregar tabla dinámica
            int index = sheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[index];

            // Obtener la conexión externa (propiedad de solo lectura)
            ExternalConnection connection = pivot.ExternalConnectionDataSource;
            
            if (connection != null)
            {
                Console.WriteLine("Pivot table connection: " + connection.Name);
            }
            else
            {
                Console.WriteLine("No external connection found");
            }
        }
    }
}
```

### Ver también

* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


