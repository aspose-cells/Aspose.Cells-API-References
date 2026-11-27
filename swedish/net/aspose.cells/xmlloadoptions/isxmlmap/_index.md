---
title: "XmlLoadOptions.IsXmlMap"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XmlLoadOptions‑egenskap. Anger om XML ska kartläggas till Excel. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/xmlloadoptions/isxmlmap/
---
## XmlLoadOptions.IsXmlMap property

Anger om xml ska mappas till Excel. Standardvärdet är falskt.

```csharp
public bool IsXmlMap { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyIsXmlMapDemo
    {
        public static void Run()
        {
            // Skapa en instans av XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Aktivera XML‑kartläggning när filen laddas
            options.IsXmlMap = true;

            // Läs in en XML-fil i en Workbook med de angivna alternativen
            Workbook workbook = new Workbook("sample.xml", options);

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Visa lite data från den laddade XML‑filen för att demonstrera lyckad kartläggning
            Console.WriteLine("Data from loaded XML:");
            Console.WriteLine(worksheet.Cells["A1"].StringValue);
            Console.WriteLine(worksheet.Cells["A2"].StringValue);

            // Spara arbetsboken till en ny Excel‑fil
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


