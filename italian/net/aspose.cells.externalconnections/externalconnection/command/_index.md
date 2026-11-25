---
title: "ExternalConnection.Command"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. La stringa contenente il comando del database da passare all'API del provider dati che interagirà con la fonte esterna per recuperare i dati"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/command/
---
## ExternalConnection.Command property

La stringa contenente il comando del database da passare all'API del provider dati che interagirà con la fonte esterna per recuperare i dati

```csharp
public virtual string Command { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro e alcuni dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(150);
            
            // Crea un intervallo di tabella
            var range = worksheet.Cells.CreateRange("A1:B3");
            
            // Crea una tabella pivot utilizzando l'intervallo come origine
            int index = worksheet.PivotTables.Add("D1", "A1:B3", "PivotTable1");
            var pivotTable = worksheet.PivotTables[index];
            
            // Ottieni le connessioni esterne
            ExternalConnection[] connections = pivotTable.GetSourceDataConnections();
            
            // Visualizza la proprietà Command della connessione
            if (connections.Length > 0)
            {
                Console.WriteLine("Connection Command: " + connections[0].Command);
            }
            
            // Salva la cartella di lavoro
            workbook.Save("ExternalConnectionCommandDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


