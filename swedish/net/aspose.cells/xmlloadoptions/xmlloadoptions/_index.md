---
title: "XmlLoadOptions.XmlLoadOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XmlLoadOptions-konstruktor. Representerar alternativen för att läsa in XML-fil"
type: docs
url: /sv/net/aspose.cells/xmlloadoptions/xmlloadoptions/
---
## XmlLoadOptions() {#constructor}

Representerar alternativen för att läsa in en XML-fil.

```csharp
public XmlLoadOptions()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa nya XML-inläsningsalternativ
            XmlLoadOptions options = new XmlLoadOptions();
            
            // Ställ in för att konvertera numeriska eller datumvärden
            options.ConvertNumericOrDate = true;
            
            // Läs in arbetsbok med alternativ
            Workbook workbook = new Workbook("input.xml", options);
            
            // Få åtkomst till celldata
            Cell cell = workbook.Worksheets[0].Cells["A1"];
            Console.WriteLine("Cell Value: " + cell.Value);
            Console.WriteLine("Cell Type: " + cell.Type);
            
            // Spara arbetsbok
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XmlLoadOptions(LoadFormat) {#constructor_1}

Representerar alternativen för att läsa in en XML-fil.

```csharp
public XmlLoadOptions(LoadFormat type)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | LoadFormat | Inläsningsformatstypen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XmlLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en XmlLoadOptions-instans med LoadFormat-parameter
                LoadFormat loadFormat = LoadFormat.Xml;
                XmlLoadOptions xmlLoadOptions = new XmlLoadOptions(loadFormat);

                // Ange några egenskaper för XmlLoadOptions
                xmlLoadOptions.StartCell = "A1";
                xmlLoadOptions.IsXmlMap = true;
                xmlLoadOptions.ConvertNumericOrDate = true;

                // Skapa en arbetsbok med laddningsalternativen
                Workbook workbook = new Workbook("sample.xml", xmlLoadOptions);

                // Åtkomst till det första kalkylbladet
                Worksheet worksheet = workbook.Worksheets[0];

                // Visa viss information
                Console.WriteLine("XML file loaded successfully with LoadFormat.Xml");
                Console.WriteLine($"First cell value: {worksheet.Cells["A1"].Value}");

                // Spara arbetsboken
                workbook.Save("XmlLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing XmlLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [LoadFormat](../../loadformat/)
* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


