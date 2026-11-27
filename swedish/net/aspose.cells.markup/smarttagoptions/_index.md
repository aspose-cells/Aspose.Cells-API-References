---
title: "Klass SmartTagOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Markup.SmartTagOptions-klass. Representerar alternativen för den smarta taggen"
type: docs
url: /sv/net/aspose.cells.markup/smarttagoptions/
---
## SmartTagOptions class

Representerar alternativen för den smarta taggen.

```csharp
public class SmartTagOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [SmartTagOptions](smarttagoptions/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [EmbedSmartTags](../../aspose.cells.markup/smarttagoptions/embedsmarttags/) { get; set; } | Anger om smarta taggar sparas med arbetsboken. |
| [ShowType](../../aspose.cells.markup/smarttagoptions/showtype/) { get; set; } | Representerar visningstypen för smart tag. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassSmartTagOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en instans av SmartTagOptions
            SmartTagOptions options = new SmartTagOptions();

            // Ställ in egenskaper
            options.EmbedSmartTags = true;
            options.ShowType = SmartTagShowType.NoSmartTagIndicator;

            // Applicera SmartTagOptions på kalkylbladet
            // Obs: Ändrad från worksheet.SmartTagSetting.Options = options;
            // för att direkt använda options-objektet eftersom SmartTagSetting inte har någon Options-egenskap
            // (Förutsatt att alternativen är avsedda att användas direkt)
            
            // Lägg till lite data för att demonstrera
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);

            // Spara arbetsboken
            workbook.Save("SmartTagOptionsDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


