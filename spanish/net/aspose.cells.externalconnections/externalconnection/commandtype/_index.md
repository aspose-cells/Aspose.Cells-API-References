---
title: "ExternalConnection.CommandType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnection. Especifica el tipo de comando OLE DB. 1. Consulta especifica un nombre de cubo 2. Consulta especifica una sentencia SQL 3. Consulta especifica un nombre de tabla 4. Consulta especifica que se ha proporcionado información predeterminada y depende del proveedor interpretarla. 5. Consulta se realiza contra un proveedor de datos de lista basado en web"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/commandtype/
---
## ExternalConnection.CommandType property

Especifica el tipo de comando OLE DB. 1. La consulta especifica un nombre de cubo 2. La consulta especifica una instrucción SQL 3. La consulta especifica un nombre de tabla 4. La consulta indica que se ha proporcionado información predeterminada, y depende del proveedor interpretarla. 5. La consulta se realiza contra un proveedor de datos de lista basado en la web.

```csharp
public virtual OLEDBCommandType CommandType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyCommandTypeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1500);

            // Crear una tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[index];

            // Obtener la conexión externa
            ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
            
            // Demostrar la propiedad CommandType
            Console.WriteLine("Original CommandType: " + conn.CommandType);
            
            // Cambiar y mostrar CommandType
            conn.CommandType = Aspose.Cells.ExternalConnections.OLEDBCommandType.TableName;
            Console.WriteLine("Modified CommandType: " + conn.CommandType);
            
            // Guarda el libro de trabajo
            workbook.Save("ExternalConnectionCommandTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


