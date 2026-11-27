---
title: "XmlLoadOptions.ConvertNumericOrDate"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XmlLoadOptions‑egenskap. Anger om värdet i XML‑filen ska konverteras till numeriskt eller datum"
type: docs
url: /sv/net/aspose.cells/xmlloadoptions/convertnumericordate/
---
## XmlLoadOptions.ConvertNumericOrDate property

Anger om värdet i xml-filen konverteras till numeriskt eller datum.

```csharp
public bool ConvertNumericOrDate { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyConvertNumericOrDateDemo
    {
        public static void Run()
        {
            // Skapa XML‑inläsningsalternativ
            XmlLoadOptions options = new XmlLoadOptions();
            
            // Ställ in ConvertNumericOrDate till true (standard)
            options.ConvertNumericOrDate = true;
            Workbook wb1 = new Workbook("input.xml", options);
            Cell cell1 = wb1.Worksheets[0].Cells["A1"];
            Console.WriteLine("With conversion (true): " + cell1.Value + " is type: " + cell1.Type);
            
            // Ställ in ConvertNumericOrDate till false
            options.ConvertNumericOrDate = false;
            Workbook wb2 = new Workbook("input.xml", options);
            Cell cell2 = wb2.Worksheets[0].Cells["A1"];
            Console.WriteLine("Without conversion (false): " + cell2.Value + " is type: " + cell2.Type);
            
            // Spara resultat
            wb1.Save("output_with_conversion.xlsx");
            wb2.Save("output_without_conversion.xlsx");
        }
    }
}
```

### Se även

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


