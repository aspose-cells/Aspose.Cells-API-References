---
title: "Enum OLEDBCommandType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ExternalConnections.OLEDBCommandType‑Enum. Gibt den OLE‑DB‑Befehlstyp an"
type: docs
url: /de/net/aspose.cells.externalconnections/oledbcommandtype/
---
## OLEDBCommandType enumeration

Gibt den OLE DB-Befehlstyp an.

```csharp
public enum OLEDBCommandType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Der Befehlstyp ist nicht angegeben. |
| CubeName | `1` | Gibt einen Würfelnamen an |
| SqlStatement | `2` | Gibt eine SQL‑Anweisung an |
| TableName | `3` | Gibt einen Tabellennamen an |
| DefaultInformation | `4` | Gibt an, dass Standardinformationen bereitgestellt wurden, und überlässt es dem Anbieter, wie diese zu interpretieren sind. |
| WebBasedList | `5` | Gibt eine Abfrage an, die gegen einen webbasierten List Data Provider gerichtet ist. |
| TableCollection | `6` | Gibt die Tabellenliste an. |

### Beispiele

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
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            // Erstelle eine Pivot-Tabelle
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Hole die externe Verbindung
            ExternalConnectionCollection connections = workbook.DataConnections;
            ExternalConnection conn = connections[0];
            
            // Demonstriere die Verwendung von OLEDBCommandType
            Console.WriteLine("Connection Name: " + conn.Name);
            Console.WriteLine("Source Type: " + conn.SourceType);
            Console.WriteLine("Command Type: " + conn.CommandType);
            Console.WriteLine("Command: " + conn.Command);
            
            // Ändere den Befehlstyp und demonstriere
            conn.CommandType = OLEDBCommandType.TableName;
            Console.WriteLine("\nAfter changing CommandType:");
            Console.WriteLine("Command Type: " + conn.CommandType);
            
            // Speichere die Arbeitsmappe
            workbook.Save("OLEDBCommandTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


