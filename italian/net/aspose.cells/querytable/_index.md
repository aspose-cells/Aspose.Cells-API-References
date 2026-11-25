---
title: "Classe QueryTable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.QueryTable. Rappresenta le informazioni di QueryTable"
type: docs
url: /it/net/aspose.cells/querytable/
---
## QueryTable class

Rappresenta le informazioni di QueryTable.

```csharp
public class QueryTable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AdjustColumnWidth](../../aspose.cells/querytable/adjustcolumnwidth/) { get; set; } | Restituisce o imposta l'AdjustColumnWidth dell'oggetto. |
| [ConnectionId](../../aspose.cells/querytable/connectionid/) { get; } | Ottiene l'ID di connessione della tabella query. |
| [ExternalConnection](../../aspose.cells/querytable/externalconnection/) { get; } | Ottiene la connessione esterna correlata. |
| [Name](../../aspose.cells/querytable/name/) { get; } | Ottiene il nome della querytable. |
| [PreserveFormatting](../../aspose.cells/querytable/preserveformatting/) { get; set; } | Restituisce o imposta il PreserveFormatting dell'oggetto. |
| [ResultRange](../../aspose.cells/querytable/resultrange/) { get; } | Ottiene l'intervallo del risultato. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassQueryTableDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per creare una tabella query (simulando dati esterni)
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");
            
            // Verifica se ci sono tabelle query nel foglio di lavoro
            if (worksheet.QueryTables.Count > 0)
            {
                // Ottieni la prima tabella query
                QueryTable qt = worksheet.QueryTables[0];
                
                // Visualizza le proprietà della tabella di query
                Console.WriteLine("Query Table Name: " + qt.Name);
                Console.WriteLine("Connection ID: " + qt.ConnectionId);
                Console.WriteLine("Result Range: " + qt.ResultRange.Address);
                Console.WriteLine("Preserve Formatting: " + qt.PreserveFormatting);
                Console.WriteLine("Adjust Column Width: " + qt.AdjustColumnWidth);
                
                // Modifica alcune proprietà
                qt.PreserveFormatting = true;
                qt.AdjustColumnWidth = false;
            }
            else
            {
                Console.WriteLine("No query tables found in the worksheet.");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


