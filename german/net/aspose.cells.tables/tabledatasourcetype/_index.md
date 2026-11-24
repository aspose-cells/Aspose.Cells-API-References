---
title: "Enum TableDataSourceType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Tables.TableDataSourceType enum. Stellt den Datentyp der Tabellen-Datenquelle dar."
type: docs
url: /de/net/aspose.cells.tables/tabledatasourcetype/
---
## TableDataSourceType enumeration

Stellt den Datentyp der Tabellen-Datenquelle dar.

```csharp
public enum TableDataSourceType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Worksheet | `0` | Excel-Arbeitsblatt-Tabelle |
| SharePoint | `1` | Lese‑Schreib‑SharePoint‑verknüpfte Liste |
| XML | `2` | XML-Mapper-Tabelle |
| QueryTable | `3` | Abfrage-Tabelle |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableDataSourceTypeDemo
    {
        public static void TableDataSourceTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);

            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue("Charlie");

            // Füge ein ListObject (Tabelle) zum Arbeitsblatt hinzu
            int listObjectIndex = worksheet.ListObjects.Add(1, 0, 4, 1, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];

            // Setzen Sie den Anzeigenamen der Tabelle
            listObject.DisplayName = "SampleTable";

            // Setzen Sie den Datentyp der Datenquelle der Tabelle
            TableDataSourceType dataSourceType = listObject.DataSourceType;

            // Geben Sie den Datentyp der Datenquelle aus
            Console.WriteLine("Data Source Type: " + dataSourceType);

            // Speichere die Arbeitsmappe
            workbook.Save("TableDataSourceTypeExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


