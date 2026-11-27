---
title: "PageSetup.PrintArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Representerar området som ska skrivas ut"
type: docs
url: /sv/net/aspose.cells/pagesetup/printarea/
---
## PageSetup.PrintArea property

Representerar det område som ska skrivas ut.

```csharp
public string PrintArea { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintAreaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(3);
            
            // Ställ in utskriftsområdet till A1:B3
            worksheet.PageSetup.PrintArea = "A1:B3";
            
            // Spara med endast utskriftsområde
            HtmlSaveOptions options = new HtmlSaveOptions
            {
                ExportPrintAreaOnly = true
            };
            
            workbook.Save("PrintAreaDemo.html", options);
            
            Console.WriteLine("Print area demo created successfully.");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


