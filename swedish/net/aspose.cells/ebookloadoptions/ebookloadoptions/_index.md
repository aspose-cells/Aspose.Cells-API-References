---
title: "EbookLoadOptions.EbookLoadOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "EbookLoadOptions-konstruktor. Skapar ett alternativ för att ladda e-bokfilen"
type: docs
url: /sv/net/aspose.cells/ebookloadoptions/ebookloadoptions/
---
## EbookLoadOptions() {#constructor}

Skapar ett alternativ för att läsa in e‑bokfilen.

```csharp
public EbookLoadOptions()
```

### Exempel

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class EbookLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en instans av EbookLoadOptions med hjälp av konstruktorn
            EbookLoadOptions options = new EbookLoadOptions();

            // Ställ in några grundläggande egenskaper
            options.Password = "secure123";
            options.Encoding = Encoding.UTF8;
            options.LoadFormulas = true;
            
            // Läs in en e-bokfil med de angivna alternativen
            Workbook workbook = new Workbook("sample.epub", options);
            
            // Spara som Excel-fil
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [EbookLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## EbookLoadOptions(LoadFormat) {#constructor_1}

Skapar ett alternativ för inläsning av e‑bokfilen.

```csharp
public EbookLoadOptions(LoadFormat loadFormat)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| loadFormat | LoadFormat | Laddningsformatet |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class EbookLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa EbookLoadOptions-instans med LoadFormat-parameter
                EbookLoadOptions options = new EbookLoadOptions(LoadFormat.Epub);

                // Visa bekräftelse
                Console.WriteLine("EbookLoadOptions created successfully with LoadFormat.Epub");

                // Exempel på användning: Ladda en arbetsbok med dessa alternativ
                Workbook workbook = new Workbook("sample.epub", options);
                Console.WriteLine("Workbook loaded successfully with EbookLoadOptions");

                // Spara resultatet
                workbook.Save("EbookLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EbookLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [LoadFormat](../../loadformat/)
* class [EbookLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


