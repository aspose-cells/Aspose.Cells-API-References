---
title: "Enum OLEDBCommandType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.ExternalConnections.OLEDBCommandType enum. Specifica il tipo di comando OLE DB"
type: docs
url: /it/net/aspose.cells.externalconnections/oledbcommandtype/
---
## OLEDBCommandType enumeration

Specifica il tipo di comando OLE DB.

```csharp
public enum OLEDBCommandType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Il tipo di comando non è specificato. |
| CubeName | `1` | Specifica un nome del cubo |
| SqlStatement | `2` | Specifica un'istruzione SQL |
| TableName | `3` | Specifica un nome della tabella |
| DefaultInformation | `4` | Specifica che sono state fornite informazioni predefinite, e spetta al provider interpretarle. |
| WebBasedList | `5` | Specifica una query che è contro un List Data Provider basato sul web. |
| TableCollection | `6` | Specifica l'elenco delle tabelle. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ExternalConnectionsClassOLEDBCommandTypeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            // Crea una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Ottieni la connessione esterna
            ExternalConnectionCollection connections = workbook.DataConnections;
            ExternalConnection conn = connections[0];
            
            // Dimostra l'uso di OLEDBCommandType
            Console.WriteLine("Connection Name: " + conn.Name);
            Console.WriteLine("Source Type: " + conn.SourceType);
            Console.WriteLine("Command Type: " + conn.CommandType);
            Console.WriteLine("Command: " + conn.Command);
            
            // Modifica il tipo di comando e dimostra
            conn.CommandType = OLEDBCommandType.TableName;
            Console.WriteLine("\nAfter changing CommandType:");
            Console.WriteLine("Command Type: " + conn.CommandType);
            
            // Salva la cartella di lavoro
            workbook.Save("OLEDBCommandTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


