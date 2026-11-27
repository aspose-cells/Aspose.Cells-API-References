---
title: "XmlSaveOptions.HasHeaderRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XmlSaveOptions-egenskap. Anger om området innehåller rubrikrad"
type: docs
url: /sv/net/aspose.cells/xmlsaveoptions/hasheaderrow/
---
## XmlSaveOptions.HasHeaderRow property

Anger om intervallet innehåller en rubrikrad.

```csharp
public bool HasHeaderRow { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertyHasHeaderRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till rubrikrad och data
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Skapa XML-sparalternativ
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.HasHeaderRow = true; // Demonstrate HasHeaderRow property
            saveOptions.SheetNameAsElementName = true;

            // Spara som XML-fil
            workbook.Save("output.xml", saveOptions);

            Console.WriteLine("XML file saved with HasHeaderRow=true");
        }
    }
}
```

### Se även

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


