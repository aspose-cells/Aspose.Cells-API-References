---
title: "Enum ConnectionDataSourceType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.ExternalConnections.ConnectionDataSourceType. Specifica il tipo di origine del database esterno"
type: docs
url: /it/net/aspose.cells.externalconnections/connectiondatasourcetype/
---
## ConnectionDataSourceType enumeration

Specifica il tipo di origine del database esterno

```csharp
public enum ConnectionDataSourceType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| ODBCBasedSource | `1` | Origine basata su ODBC |
| DAOBasedSource | `2` | Origine basata su DAO |
| FileBasedDataBaseSource | `3` | Origine del database basata su file |
| WebQuery | `4` | Query web |
| OLEDBBasedSource | `5` | Origine basata su OLE DB |
| TextBasedSource | `6` | Origine basata su testo |
| ADORecordSet | `7` | Set di record ADO |
| DSP | `8` | DSP |
| OLEDBDataModel | `100` | Origine dati OLE DB creata dal modello di dati del foglio di calcolo. |
| DataFeedDataModel | `101` | Origine dati feed di dati creata dal modello di dati del foglio di calcolo. |
| WorksheetDataModel | `102` | Origine dati del foglio di lavoro creata dal modello di dati del foglio di calcolo. |
| Table | `102` | Origine dati del foglio di lavoro creata dal modello di dati del foglio di calcolo. |
| TextDataModel | `103` | Origine dati di testo creata dal modello di dati del foglio di calcolo. |
| Unknown | `255` | Origine dati di testo creata dal modello di dati del foglio di calcolo. |

### Esempi

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
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio al foglio di lavoro
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["B3"].PutValue(2000);

            // Crea una tabella pivot utilizzando i dati del foglio di lavoro
            var pivotTable = sheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            
            // Ottieni la connessione e dimostra ConnectionDataSourceType
            var conn = sheet.PivotTables[0].GetSourceDataConnections()[0];
            Console.WriteLine("Connection Name: " + conn.Name);
            Console.WriteLine("Class Type: " + conn.ClassType);
            Console.WriteLine("Source Type: " + conn.SourceType);
            Console.WriteLine("Command: " + conn.Command);
            
            // Salva la cartella di lavoro
            workbook.Save("ExternalConnectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


