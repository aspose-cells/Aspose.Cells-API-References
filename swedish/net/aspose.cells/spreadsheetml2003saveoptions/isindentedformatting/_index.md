---
title: "SpreadsheetML2003SaveOptions.IsIndentedFormatting"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SpreadsheetML2003SaveOptions egenskap. Gör att underordnade element indenteras"
type: docs
url: /sv/net/aspose.cells/spreadsheetml2003saveoptions/isindentedformatting/
---
## SpreadsheetML2003SaveOptions.IsIndentedFormatting property

Gör så att underordnade element indenteras.

```csharp
public bool IsIndentedFormatting { get; set; }
```

### Anmärkningar

Standardvärdet är true. Om värdet är false minskar det filens xml-storlek

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsPropertyIsIndentedFormattingDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);

            // Konfigurera sparalternativ med indenterad formatering
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions
            {
                IsIndentedFormatting = true
            };

            // Spara med indenterad XML-formatering
            workbook.Save("output_indented.xml", saveOptions);

            // Spara utan indenterad formatering för jämförelse
            saveOptions.IsIndentedFormatting = false;
            workbook.Save("output_not_indented.xml", saveOptions);
        }
    }
}
```

### Se även

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


