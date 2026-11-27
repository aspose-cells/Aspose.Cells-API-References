---
title: "Enum OLEDBCommandType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ExternalConnections.OLEDBCommandType‑enum. Anger OLE DB‑kommandotypen"
type: docs
url: /sv/net/aspose.cells.externalconnections/oledbcommandtype/
---
## OLEDBCommandType enumeration

Anger OLE DB-kommandotypen.

```csharp
public enum OLEDBCommandType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Kommandotypen är inte angiven. |
| CubeName | `1` | Anger ett kubnamn |
| SqlStatement | `2` | Anger ett SQL‑uttryck |
| TableName | `3` | Anger ett tabellnamn |
| DefaultInformation | `4` | Anger att standardinformation har givits, och det är upp till leverantören hur den ska tolkas. |
| WebBasedList | `5` | Anger en fråga som är mot en webb‑baserad List Data Provider. |
| TableCollection | `6` | Anger tabellistan. |

### Exempel

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
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            // Skapa en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Hämta den externa anslutningen
            ExternalConnectionCollection connections = workbook.DataConnections;
            ExternalConnection conn = connections[0];
            
            // Demonstrera användning av OLEDBCommandType
            Console.WriteLine("Connection Name: " + conn.Name);
            Console.WriteLine("Source Type: " + conn.SourceType);
            Console.WriteLine("Command Type: " + conn.CommandType);
            Console.WriteLine("Command: " + conn.Command);
            
            // Ändra kommandotyp och demonstrera
            conn.CommandType = OLEDBCommandType.TableName;
            Console.WriteLine("\nAfter changing CommandType:");
            Console.WriteLine("Command Type: " + conn.CommandType);
            
            // Spara arbetsboken
            workbook.Save("OLEDBCommandTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


