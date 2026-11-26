---
title: "DBConnection.SeverCommand"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DBConnection. Especifica una segunda cadena de texto de comando que se conserva cuando los campos de página basados en servidor de PivotTable están en uso. Para conexiones ODBC, serverCommand suele ser una consulta más amplia que command; no hay cláusula WHERE presente en la primera. Con base en estos 2 comandos, Command y ServerCommand, la interfaz de parámetros puede ser poblada y pueden construirse consultas parametrizadas"
type: docs
url: /es/net/aspose.cells.externalconnections/dbconnection/severcommand/
---
## DBConnection.SeverCommand property

Especifica una segunda cadena de texto de comando que se conserva cuando se utilizan campos de página basados en servidor de PivotTable. Para conexiones ODBC, serverCommand suele ser una consulta más amplia que command (no hay cláusula WHERE presente en la primera). Basado en estos 2 comandos (Command y ServerCommand), la interfaz de usuario de parámetros puede poblarse y pueden construirse consultas parametrizadas

```csharp
[Obsolete("Use ExternalConnection.SecondCommand property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string SeverCommand { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad ExternalConnection.SecondCommand. Este método será eliminado 12 meses después, a partir de octubre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class DBConnectionPropertySeverCommandDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook("input.xlsx");
            ExternalConnectionCollection connections = workbook.DataConnections;

            foreach (ExternalConnection connection in connections)
            {
                if (connection is DBConnection dbConn)
                {
                    dbConn.Name = dbConn.Name.Replace("c:\\", "d:\\");
                    dbConn.SourceFile = dbConn.SourceFile.Replace("c:\\", "d:\\");
                    dbConn.ConnectionInfo = dbConn.ConnectionInfo.Replace("c:\\", "d:\\").Replace("C:\\", "d:\\");
                    dbConn.Command = dbConn.Command.Replace("c:\\", "d:\\");
                    
                    if (!string.IsNullOrEmpty(dbConn.SeverCommand))
                        dbConn.SeverCommand = dbConn.SeverCommand.Replace("c:\\", "d:\\");
                }
            }

            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


