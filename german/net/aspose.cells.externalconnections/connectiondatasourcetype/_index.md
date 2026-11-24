---
title: "Enum ConnectionDataSourceType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ExternalConnections.ConnectionDataSourceType Enum. Gibt den Typ der externen Datenbankquelle an."
type: docs
url: /de/net/aspose.cells.externalconnections/connectiondatasourcetype/
---
## ConnectionDataSourceType enumeration

Gibt den Typ der externen Datenbankquelle an

```csharp
public enum ConnectionDataSourceType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| ODBCBasedSource | `1` | ODBC-basierte Quelle |
| DAOBasedSource | `2` | DAO-basierte Quelle |
| FileBasedDataBaseSource | `3` | Dateibasierte Datenbankquelle |
| WebQuery | `4` | Webabfrage |
| OLEDBBasedSource | `5` | OLE DB-basierte Quelle |
| TextBasedSource | `6` | Textbasierte Quelle |
| ADORecordSet | `7` | ADO-Datensatz |
| DSP | `8` | DSP |
| OLEDBDataModel | `100` | OLE DB-Datenquelle, erstellt vom Spreadsheet-Datenmodell. |
| DataFeedDataModel | `101` | Data-Feed-Datenquelle, erstellt vom Spreadsheet-Datenmodell. |
| WorksheetDataModel | `102` | Arbeitsblatt-Datenquelle, erstellt vom Spreadsheet-Datenmodell. |
| Table | `102` | Arbeitsblatt-Datenquelle, erstellt vom Spreadsheet-Datenmodell. |
| TextDataModel | `103` | Textdatenquelle, erstellt vom Spreadsheet-Datenmodell. |
| Unknown | `255` | Textdatenquelle, erstellt vom Spreadsheet-Datenmodell. |

### Beispiele

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
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Arbeitsblatt hinzufügen
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["B3"].PutValue(2000);

            // Erstelle eine Pivot-Tabelle mit den Arbeitsblattdaten
            var pivotTable = sheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            
            // Hole die Verbindung und demonstriere ConnectionDataSourceType
            var conn = sheet.PivotTables[0].GetSourceDataConnections()[0];
            Console.WriteLine("Connection Name: " + conn.Name);
            Console.WriteLine("Class Type: " + conn.ClassType);
            Console.WriteLine("Source Type: " + conn.SourceType);
            Console.WriteLine("Command: " + conn.Command);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ExternalConnectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


