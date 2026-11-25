---
title: "DBConnection.SeverCommand"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DBConnection. Specifica una seconda stringa di testo del comando che viene mantenuta quando i campi pagina basati su server di PivotTable sono in uso. Per le connessioni ODBC serverCommand è solitamente una query più ampia rispetto a command, poiché nella prima non è presente la clausola WHERE. Sulla base di questi due comandi, Command e ServerCommand, l'interfaccia dei parametri può essere popolata e possono essere costruite query parametrizzate"
type: docs
url: /it/net/aspose.cells.externalconnections/dbconnection/severcommand/
---
## DBConnection.SeverCommand property

Specifica una seconda stringa di testo del comando che viene mantenuta quando i campi di pagina basati su server della PivotTable sono in uso. Per le connessioni ODBC, serverCommand è solitamente una query più ampia rispetto a command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed

```csharp
[Obsolete("Use ExternalConnection.SecondCommand property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string SeverCommand { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà ExternalConnection.SecondCommand. Questo metodo sarà rimosso tra 12 mesi a partire da ottobre 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

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

### Vedi anche

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


