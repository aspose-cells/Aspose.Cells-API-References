---
title: "XmlLoadOptions.DateFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XmlLoadOptions-egenskap. Hämtar och anger formatet för datumvärde"
type: docs
url: /sv/net/aspose.cells/xmlloadoptions/dateformat/
---
## XmlLoadOptions.DateFormat property

Hämtar och anger formatet för datumvärdet.

```csharp
public string DateFormat { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyDateFormatDemo
    {
        public static void Run()
        {
            // Skapa en instans av XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Ange datumformatet för att tolka datum från XML
            options.DateFormat = "yyyy-MM-dd";
            options.ConvertNumericOrDate = true;

            // Läs in en XML-fil i en Workbook med de angivna alternativen
            Workbook workbook = new Workbook("input.xml", options);

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Visa några celler för att demonstrera datumformatering
            Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].Value);

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


