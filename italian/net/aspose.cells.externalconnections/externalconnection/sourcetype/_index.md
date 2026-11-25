---
title: "ExternalConnection.SourceType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. Ottiene o imposta il tipo di DataSource della connessione esterna"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/sourcetype/
---
## ExternalConnection.SourceType property

Ottiene o imposta il tipo di DataSource della connessione esterna.

```csharp
public ConnectionDataSourceType SourceType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertySourceTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro e crea una tabella pivot
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["B3"].PutValue(2000);
            
            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B3", "C3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];
            
            // Ottieni la connessione esterna
            ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
            
            // Dimostra la proprietà SourceType
            Console.WriteLine("Connection Source Type: " + conn.SourceType);
            
            // Modifica le proprietà della connessione
            conn.Name = "TestConnection";
            conn.SourceType = ConnectionDataSourceType.OLEDBDataModel;
            
            // Visualizza le proprietà modificate
            Console.WriteLine("Modified Connection Name: " + conn.Name);
            Console.WriteLine("Modified Source Type: " + conn.SourceType);
        }
    }
}
```

### Vedi anche

* enum [ConnectionDataSourceType](../../connectiondatasourcetype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


