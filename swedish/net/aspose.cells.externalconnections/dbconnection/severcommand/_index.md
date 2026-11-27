---
title: "DBConnection.SeverCommand"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DBConnection egenskap. Specificerar en andra kommandotextsträng som sparas när PivotTable‑serverbaserade sidfält används. För ODBC‑anslutningar är serverCommand vanligtvis en bredare fråga än command; ingen WHERE‑klausul finns i den förra. Baserat på dessa två kommandon, Command och ServerCommand, kan parameter‑UI fyllas i och parametriserade frågor kan konstrueras."
type: docs
url: /sv/net/aspose.cells.externalconnections/dbconnection/severcommand/
---
## DBConnection.SeverCommand property

Anger en andra kommandotextsträng som bevaras när PivotTable-serverbaserade sidfält används. För ODBC-anslutningar är serverCommand vanligtvis en bredare fråga än command (ingen WHERE-klausul finns i den förra). Baserat på dessa två kommandon (Command och ServerCommand) kan parameter‑UI fyllas i och parametriserade frågor konstrueras

```csharp
[Obsolete("Use ExternalConnection.SecondCommand property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string SeverCommand { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället ExternalConnection.SecondCommand‑egenskapen. Denna metod kommer att tas bort 12 månader senare från och med oktober 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

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

### Se även

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


