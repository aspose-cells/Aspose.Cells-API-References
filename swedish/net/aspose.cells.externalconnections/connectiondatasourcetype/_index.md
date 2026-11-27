---
title: "Enum ConnectionDataSourceType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ExternalConnections.ConnectionDataSourceType enum. Anger typ av extern databaskälla"
type: docs
url: /sv/net/aspose.cells.externalconnections/connectiondatasourcetype/
---
## ConnectionDataSourceType enumeration

Anger typ av extern databaskälla

```csharp
public enum ConnectionDataSourceType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| ODBCBasedSource | `1` | ODBC-baserad källa |
| DAOBasedSource | `2` | DAO-baserad källa |
| FileBasedDataBaseSource | `3` | Filbaserad databaskälla |
| WebQuery | `4` | Web‑fråga |
| OLEDBBasedSource | `5` | OLE DB-baserad källa |
| TextBasedSource | `6` | Textbaserad källa |
| ADORecordSet | `7` | ADO‑postuppsättning |
| DSP | `8` | DSP |
| OLEDBDataModel | `100` | OLE DB-datakälla skapad av Spreadsheet Data Model. |
| DataFeedDataModel | `101` | Dataflödesdatakälla skapad av Spreadsheet Data Model. |
| WorksheetDataModel | `102` | Arbetsbladsdatakälla skapad av kalkylbladsdatamodellen. |
| Table | `102` | Arbetsbladsdatakälla skapad av kalkylbladsdatamodellen. |
| TextDataModel | `103` | Textdatakälla skapad av kalkylbladsdatamodellen. |
| Unknown | `255` | Textdatakälla skapad av kalkylbladsdatamodellen. |

### Exempel

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
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i arbetsbladet
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["B3"].PutValue(2000);

            // Skapa en pivottabell med arbetsbladsdata
            var pivotTable = sheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            
            // Hämta anslutningen och demonstrera ConnectionDataSourceType
            var conn = sheet.PivotTables[0].GetSourceDataConnections()[0];
            Console.WriteLine("Connection Name: " + conn.Name);
            Console.WriteLine("Class Type: " + conn.ClassType);
            Console.WriteLine("Source Type: " + conn.SourceType);
            Console.WriteLine("Command: " + conn.Command);
            
            // Spara arbetsboken
            workbook.Save("ExternalConnectionDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


