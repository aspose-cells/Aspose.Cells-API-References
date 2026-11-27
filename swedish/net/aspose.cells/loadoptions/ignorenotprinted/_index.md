---
title: "LoadOptions.IgnoreNotPrinted"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadOptions-egenskap. Ignorera data som inte skrivs ut om filen skrivs ut direkt"
type: docs
url: /sv/net/aspose.cells/loadoptions/ignorenotprinted/
---
## LoadOptions.IgnoreNotPrinted property

Ignorera data som inte skrivs ut om filen skrivs ut direkt.

```csharp
public bool IgnoreNotPrinted { get; set; }
```

### Anmärkningar

Endast för xlsx-fil.

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyIgnoreNotPrintedDemo
    {
        public static void Run()
        {
            // Skapa HTML-inläsningsalternativ och ange IgnoreNotPrinted
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.AutoFitColsAndRows = true;

            // Läs in HTML-fil med de angivna alternativen
            Workbook workbook = new Workbook("example.html", loadOptions);
            Worksheet worksheet = workbook.Worksheets[0];

            // Visa effekten av IgnoreNotPrinted genom att kontrollera cellstilar
            Console.WriteLine("B3 Cell Color: " + worksheet.Cells["B3"].GetStyle().ForegroundColor);
            Console.WriteLine("B4 Cell Color: " + worksheet.Cells["B4"].GetStyle().ForegroundColor);
            Console.WriteLine("B5 Cell Color: " + worksheet.Cells["B5"].GetStyle().ForegroundColor);

            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


