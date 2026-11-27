---
title: "OdsLoadOptions.ApplyExcelDefaultStyleToHyperlink"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OdsLoadOptions egenskap. Anger om standardstilen i Excel ska tillämpas på hyperlänk"
type: docs
url: /sv/net/aspose.cells/odsloadoptions/applyexceldefaultstyletohyperlink/
---
## OdsLoadOptions.ApplyExcelDefaultStyleToHyperlink property

Anger om standardstilen i Excel ska tillämpas på hyperlänken.

```csharp
public bool ApplyExcelDefaultStyleToHyperlink { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OdsLoadOptionsPropertyApplyExcelDefaultStyleToHyperlinkDemo
    {
        public static void Run()
        {
            // Skapa en instans av OdsLoadOptions
            OdsLoadOptions loadOptions = new OdsLoadOptions();

            // Ange ApplyExcelDefaultStyleToHyperlink egenskap
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;

            // Läs in en ODS-fil med de angivna alternativen
            Workbook workbook = new Workbook("sample.ods", loadOptions);

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en hyperlänk för att demonstrera stilens tillämpning
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            // Spara arbetsboken till en ny fil
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


