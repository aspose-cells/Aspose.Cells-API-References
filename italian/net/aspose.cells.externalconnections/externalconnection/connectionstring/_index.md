---
title: "ExternalConnection.ConnectionString"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. La stringa di informazioni di connessione è usata per stabilire un contatto con una fonte dati OLE DB o ODBC"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/connectionstring/
---
## ExternalConnection.ConnectionString property

La stringa di informazioni della connessione è usata per contattare una fonte dati OLE DB o ODBC.

```csharp
public virtual string ConnectionString { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyConnectionStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea dati di esempio
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1500);
            
            // Crea una tabella pivot
            int index = worksheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Ottieni le connessioni dati
            ExternalConnection[] connections = pivotTable.GetSourceDataConnections();
            
            // Visualizza la stringa di connessione se esiste
            if (connections.Length > 0)
            {
                Console.WriteLine("Connection String: " + connections[0].ConnectionString);
            }
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableWithConnection.xlsx");
        }
    }
}
```

### Vedi anche

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


