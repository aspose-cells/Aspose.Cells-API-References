---
title: "PivotTable.ExternalConnectionDataSource"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Ottiene la fonte dati della connessione esterna"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/externalconnectiondatasource/
---
## PivotTable.ExternalConnectionDataSource property

Ottiene la fonte dati della connessione esterna.

```csharp
[Obsolete("Use PivotTable.GetSourceDataConnections() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ExternalConnection ExternalConnectionDataSource { get; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare il metodo PivotTable.GetSourceDataConnections(). Questo metodo sarà rimosso 12 mesi dopo, a partire da ottobre 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyExternalConnectionDataSourceDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con connessione dati esterna
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Crea dati di esempio
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["B3"].PutValue(2000);

            // Aggiungi tabella pivot
            int index = sheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[index];

            // Ottieni la connessione esterna (proprietà di sola lettura)
            ExternalConnection connection = pivot.ExternalConnectionDataSource;
            
            if (connection != null)
            {
                Console.WriteLine("Pivot table connection: " + connection.Name);
            }
            else
            {
                Console.WriteLine("No external connection found");
            }
        }
    }
}
```

### Vedi anche

* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


