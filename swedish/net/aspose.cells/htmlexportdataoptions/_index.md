---
title: "Enum HtmlExportDataOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.HtmlExportDataOptions‑enum. Representerar alternativen för export av HTML‑data"
type: docs
url: /sv/net/aspose.cells/htmlexportdataoptions/
---
## HtmlExportDataOptions enumeration

Representerar alternativen för att exportera HTML-data.

```csharp
public enum HtmlExportDataOptions
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Table | `1` | Exportera fil till HTML som endast innehåller tabelldelen. |
| All | `255` | Exportera all data till HTML. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlExportDataOptionsDemo
    {
        public static void HtmlExportDataOptionsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John Doe");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane Doe");
            worksheet.Cells["B3"].PutValue(25);

            // Skapa HtmlSaveOptions och ange HtmlExportDataOptions
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportDataOptions = HtmlExportDataOptions.All; // Export all data to HTML

            // Spara arbetsboken i HTML-format
            workbook.Save("HtmlExportDataOptionsExample_All.html", saveOptions);

            // Ändra HtmlExportDataOptions så att endast tabelldelen exporteras
            saveOptions.ExportDataOptions = HtmlExportDataOptions.Table; // Export only the table part

            // Spara arbetsboken i HTML-format igen
            workbook.Save("HtmlExportDataOptionsExample_Table.html", saveOptions);

            Console.WriteLine("HTML files have been saved successfully.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


