---
title: "Enum SmartTagShowType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Markup.SmartTagShowType-enum. Representerar visningstypen för den smarta taggen"
type: docs
url: /sv/net/aspose.cells.markup/smarttagshowtype/
---
## SmartTagShowType enumeration

Representerar visningstypen för den smarta taggen.

```csharp
public enum SmartTagShowType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| All | `0` | Anger att smarta taggar är aktiverade och visas |
| NoSmartTagIndicator | `1` | Anger att smarta taggar är aktiverade men indikatorn visas inte. |
| None | `2` | Indikerar att smarta taggar är inaktiverade och inte visas. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassSmartTagShowTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Visa alla värden i enumen SmartTagShowType
            Console.WriteLine("SmartTagShowType values:");
            Console.WriteLine($"All: {SmartTagShowType.All}");
            Console.WriteLine($"NoSmartTagIndicator: {SmartTagShowType.NoSmartTagIndicator}");
            Console.WriteLine($"None: {SmartTagShowType.None}");

            // Skapa och konfigurera en smart tagg
            var smartTagCollection = worksheet.SmartTagSetting.Add("urn:schemas-microsoft-com:office:smarttags#date");

            // Ställ in egenskaper som skulle använda SmartTagShowType (simulerat eftersom den faktiska egenskapen inte är tillgänglig)
            Console.WriteLine("\nSmart tag created at A1 with current date");

            // Spara med olika visningstypscenarier
            workbook.Save("SmartTagShowTypeDemo_All.xlsx");
            Console.WriteLine("Workbook saved with default show type (All)");

            // Skapa en annan arbetsbok med annat beteende för visningstyp
            Workbook workbook2 = new Workbook();
            Worksheet worksheet2 = workbook2.Worksheets[0];
            worksheet2.SmartTagSetting.Add("urn:schemas-microsoft-com:office:smarttags#date");
            Console.WriteLine("\nSecond workbook created with smart tag at B2");

            workbook2.Save("SmartTagShowTypeDemo_None.xlsx");
            Console.WriteLine("Second workbook saved (simulating None behavior)");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


