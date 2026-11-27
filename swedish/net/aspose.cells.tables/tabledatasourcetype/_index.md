---
title: "Enum TableDataSourceType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Tables.TableDataSourceType enum. Representerar tabellens datakälltyp"
type: docs
url: /sv/net/aspose.cells.tables/tabledatasourcetype/
---
## TableDataSourceType enumeration

Representerar tabellens datakälltyp.

```csharp
public enum TableDataSourceType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Worksheet | `0` | Excel arbetsbladstabell |
| SharePoint | `1` | Läs‑skriv SharePoint‑länkad lista |
| XML | `2` | XML‑mapper‑tabell |
| QueryTable | `3` | Frågetabell |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);

            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue("Charlie");

            // Lägg till ett ListObject (tabell) i kalkylbladet
            int listObjectIndex = worksheet.ListObjects.Add(1, 0, 4, 1, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];

            // Ställ in visningsnamnet för tabellen
            listObject.DisplayName = "SampleTable";

            // Ställ in datakälltyp för tabellen
            TableDataSourceType dataSourceType = listObject.DataSourceType;

            // Mata ut datakälltypen
            Console.WriteLine("Data Source Type: " + dataSourceType);

            // Spara arbetsboken
            workbook.Save("TableDataSourceTypeExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


