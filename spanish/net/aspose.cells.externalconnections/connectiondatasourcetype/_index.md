---
title: "Enumeración ConnectionDataSourceType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.ExternalConnections.ConnectionDataSourceType. Especifica el tipo de origen de base de datos externa"
type: docs
url: /es/net/aspose.cells.externalconnections/connectiondatasourcetype/
---
## ConnectionDataSourceType enumeration

Especifica el tipo de origen de base de datos externa

```csharp
public enum ConnectionDataSourceType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| ODBCBasedSource | `1` | Origen basado en ODBC |
| DAOBasedSource | `2` | Origen basado en DAO |
| FileBasedDataBaseSource | `3` | Origen de base de datos basado en archivo |
| WebQuery | `4` | Consulta web |
| OLEDBBasedSource | `5` | Origen basado en OLE DB |
| TextBasedSource | `6` | Origen basado en texto |
| ADORecordSet | `7` | Conjunto de registros ADO |
| DSP | `8` | DSP |
| OLEDBDataModel | `100` | Origen de datos OLE DB creado por el modelo de datos de la hoja de cálculo. |
| DataFeedDataModel | `101` | Origen de datos de alimentación creado por el modelo de datos de la hoja de cálculo. |
| WorksheetDataModel | `102` | Origen de datos de hoja de cálculo creado por el modelo de datos de la hoja de cálculo. |
| Table | `102` | Origen de datos de hoja de cálculo creado por el modelo de datos de la hoja de cálculo. |
| TextDataModel | `103` | Origen de datos de texto creado por el modelo de datos de la hoja de cálculo. |
| Unknown | `255` | Origen de datos de texto creado por el modelo de datos de la hoja de cálculo. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionsClassConnectionDataSourceTypeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a la hoja de cálculo
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["B3"].PutValue(2000);

            // Crear una tabla dinámica usando los datos de la hoja de cálculo
            var pivotTable = sheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            
            // Obtener la conexión y demostrar ConnectionDataSourceType
            var conn = sheet.PivotTables[0].GetSourceDataConnections()[0];
            Console.WriteLine("Connection Name: " + conn.Name);
            Console.WriteLine("Class Type: " + conn.ClassType);
            Console.WriteLine("Source Type: " + conn.SourceType);
            Console.WriteLine("Command: " + conn.Command);
            
            // Guarda el libro de trabajo
            workbook.Save("ExternalConnectionDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


