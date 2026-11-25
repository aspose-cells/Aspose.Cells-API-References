---
title: "ExternalConnection.CommandType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. Specifica il tipo di comando OLE DB. 1. Query specifica un nome di cubo 2. Query specifica un'istruzione SQL 3. Query specifica un nome di tabella 4. Query specifica che sono state fornite informazioni predefinite ed è compito del provider interpretarle. 5. Query è contro un provider di dati elenco basato sul web"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/commandtype/
---
## ExternalConnection.CommandType property

Specifica il tipo di comando OLE DB. 1. La query specifica un nome di cubo 2. La query specifica un'istruzione SQL 3. La query specifica un nome di tabella 4. La query specifica che sono state fornite informazioni predefinite, e spetta al provider interpretarle. 5. La query è rivolta a un provider di dati elenco basato sul web.

```csharp
public virtual OLEDBCommandType CommandType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyCommandTypeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1500);

            // Crea una tabella pivot
            int index = worksheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[index];

            // Ottieni la connessione esterna
            ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
            
            // Dimostra la proprietà CommandType
            Console.WriteLine("Original CommandType: " + conn.CommandType);
            
            // Modifica e mostra CommandType
            conn.CommandType = Aspose.Cells.ExternalConnections.OLEDBCommandType.TableName;
            Console.WriteLine("Modified CommandType: " + conn.CommandType);
            
            // Salva la cartella di lavoro
            workbook.Save("ExternalConnectionCommandTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


