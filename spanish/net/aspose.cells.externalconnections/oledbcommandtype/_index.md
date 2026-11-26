---
title: "Enum OLEDBCommandType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.ExternalConnections.OLEDBCommandType. Especifica el tipo de comando OLE DB"
type: docs
url: /es/net/aspose.cells.externalconnections/oledbcommandtype/
---
## OLEDBCommandType enumeration

Especifica el tipo de comando OLE DB.

```csharp
public enum OLEDBCommandType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | El tipo de comando no está especificado. |
| CubeName | `1` | Especifica un nombre de cubo |
| SqlStatement | `2` | Especifica una instrucción SQL |
| TableName | `3` | Especifica un nombre de tabla |
| DefaultInformation | `4` | Especifica que se ha proporcionado información predeterminada, y depende del proveedor interpretarla. |
| WebBasedList | `5` | Especifica una consulta que se realiza contra un proveedor de datos de lista basado en la web. |
| TableCollection | `6` | Especifica la lista de tablas. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ExternalConnectionsClassOLEDBCommandTypeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            // Crear una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Obtener la conexión externa
            ExternalConnectionCollection connections = workbook.DataConnections;
            ExternalConnection conn = connections[0];
            
            // Demostrar el uso de OLEDBCommandType
            Console.WriteLine("Connection Name: " + conn.Name);
            Console.WriteLine("Source Type: " + conn.SourceType);
            Console.WriteLine("Command Type: " + conn.CommandType);
            Console.WriteLine("Command: " + conn.Command);
            
            // Cambiar el tipo de comando y demostrar
            conn.CommandType = OLEDBCommandType.TableName;
            Console.WriteLine("\nAfter changing CommandType:");
            Console.WriteLine("Command Type: " + conn.CommandType);
            
            // Guarda el libro de trabajo
            workbook.Save("OLEDBCommandTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


