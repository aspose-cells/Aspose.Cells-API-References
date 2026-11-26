---
title: "ExternalConnection.Command"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnection. La cadena que contiene el comando de base de datos para pasar a la API del proveedor de datos que interactuará con la fuente externa para recuperar datos"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/command/
---
## ExternalConnection.Command property

La cadena que contiene el comando de base de datos que se pasa a la API del proveedor de datos que interactuará con la fuente externa para recuperar datos

```csharp
public virtual string Command { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyCommandDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo y algunos datos de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(150);
            
            // Crear un rango de tabla
            var range = worksheet.Cells.CreateRange("A1:B3");
            
            // Crear una tabla dinámica usando el rango como origen
            int index = worksheet.PivotTables.Add("D1", "A1:B3", "PivotTable1");
            var pivotTable = worksheet.PivotTables[index];
            
            // Obtener las conexiones externas
            ExternalConnection[] connections = pivotTable.GetSourceDataConnections();
            
            // Mostrar la propiedad Command de la conexión
            if (connections.Length > 0)
            {
                Console.WriteLine("Connection Command: " + connections[0].Command);
            }
            
            // Guarda el libro de trabajo
            workbook.Save("ExternalConnectionCommandDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


