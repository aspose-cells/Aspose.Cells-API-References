---
title: "HtmlLoadOptions.HasFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlLoadOptions‑egenskapen. Anger om texten är en formel om den börjar med"
type: docs
url: /sv/net/aspose.cells/htmlloadoptions/hasformula/
---
## HtmlLoadOptions.HasFormula property

Anger om texten är en formel om den börjar med "=".

```csharp
public bool HasFormula { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            // Skapa HTML‑laddningsalternativ
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            
            // Ställ in HasFormula till false för att behandla formelsträngar som vanlig text
            loadOptions.HasFormula = false;
            
            // Skapa arbetsbok med HTML-fil och laddningsalternativ
            Workbook workbook = new Workbook("example.html", loadOptions);
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Visa några cellvärden för att demonstrera HTML-import
            Console.WriteLine("A1: " + cells["A1"].StringValue);
            Console.WriteLine("B1: " + cells["B1"].StringValue);
            
            // Spara som XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


