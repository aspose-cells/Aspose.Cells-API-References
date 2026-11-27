---
title: "XmlLoadOptions.IgnoreRootAttributes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XmlLoadOptions‑egenskap. Anger om attribut för rotnoden ska ignoreras"
type: docs
url: /sv/net/aspose.cells/xmlloadoptions/ignorerootattributes/
---
## XmlLoadOptions.IgnoreRootAttributes property

Anger om attribut för rot-elementet ska ignoreras.

```csharp
public bool IgnoreRootAttributes { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyIgnoreRootAttributesDemo
    {
        public static void Run()
        {
            // Skapa XML‑laddningsalternativ och sätt IgnoreRootAttributes
            XmlLoadOptions options = new XmlLoadOptions();
            options.IgnoreRootAttributes = true;

            // Läs in XML-fil med alternativen
            Workbook workbook = new Workbook("example.xml", options);

            // Få åtkomst till data från den inlästa XML-filen
            string cellValue = workbook.Worksheets[0].Cells["AH8"].StringValue;
            Console.WriteLine("Cell AH8 value: " + cellValue);

            // Spara som XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


