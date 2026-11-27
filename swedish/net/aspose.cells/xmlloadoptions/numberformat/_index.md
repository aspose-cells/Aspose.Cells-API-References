---
title: "XmlLoadOptions.NumberFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XmlLoadOptions-egenskap. Hämtar och anger formatet för numeriska värden"
type: docs
url: /sv/net/aspose.cells/xmlloadoptions/numberformat/
---
## XmlLoadOptions.NumberFormat property

Hämtar och anger formatet för numeriskt värde.

```csharp
public string NumberFormat { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyNumberFormatDemo
    {
        public static void Run()
        {
            // Skapa en instans av XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Ange NumberFormat‑egenskapen för att visa tal med 2 decimaler
            options.NumberFormat = "0.00";

            // Läs in en XML-fil i en Workbook med de angivna alternativen
            Workbook workbook = new Workbook("input.xml", options);

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange några numeriska värden för att demonstrera talformatering
            worksheet.Cells["A1"].PutValue(123);
            worksheet.Cells["A2"].PutValue(45.678);
            worksheet.Cells["A3"].PutValue(0.5);

            // Spara arbetsboken till en ny fil
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


