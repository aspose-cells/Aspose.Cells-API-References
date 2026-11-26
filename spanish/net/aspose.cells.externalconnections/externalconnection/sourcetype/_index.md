---
title: "ExternalConnection.SourceType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnection. Obtiene o establece el tipo de origen de datos de la conexión externa"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/sourcetype/
---
## ExternalConnection.SourceType property

Obtiene o establece el tipo de DataSource de la conexión externa.

```csharp
public ConnectionDataSourceType SourceType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertySourceTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo y crear una tabla dinámica
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["B3"].PutValue(2000);
            
            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B3", "C3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];
            
            // Obtener la conexión externa
            ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
            
            // Demostrar la propiedad SourceType
            Console.WriteLine("Connection Source Type: " + conn.SourceType);
            
            // Modificar las propiedades de la conexión
            conn.Name = "TestConnection";
            conn.SourceType = ConnectionDataSourceType.OLEDBDataModel;
            
            // Mostrar las propiedades modificadas
            Console.WriteLine("Modified Connection Name: " + conn.Name);
            Console.WriteLine("Modified Source Type: " + conn.SourceType);
        }
    }
}
```

### Ver también

* enum [ConnectionDataSourceType](../../connectiondatasourcetype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


