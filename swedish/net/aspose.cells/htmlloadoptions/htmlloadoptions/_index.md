---
title: "HtmlLoadOptions.HtmlLoadOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlLoadOptions-konstruktorn. Skapar ett alternativ för att ladda filen"
type: docs
url: /sv/net/aspose.cells/htmlloadoptions/htmlloadoptions/
---
## HtmlLoadOptions() {#constructor}

Skapar alternativ för att läsa in filen.

```csharp
public HtmlLoadOptions()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa HTML‑laddningsalternativ med hjälp av konstruktorn
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.SupportDivTag = true;

            // Ladda HTML‑fil med alternativen
            Workbook workbook = new Workbook("example.html", loadOptions);

            // Åtkomst till data från den laddade HTML‑en
            Worksheet worksheet = workbook.Worksheets[0];
            Console.WriteLine("B1 Cell Value: " + worksheet.Cells["B1"].StringValue);
            Console.WriteLine("B3 Cell Value: " + worksheet.Cells["B3"].StringValue);
            Console.WriteLine("B4 Cell Value: " + worksheet.Cells["B4"].StringValue);
        }
    }
}
```

### Se även

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HtmlLoadOptions(LoadFormat) {#constructor_1}

Skapar alternativ för att läsa in filen.

```csharp
public HtmlLoadOptions(LoadFormat loadFormat)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| loadFormat | LoadFormat | Laddningsformatet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en HtmlLoadOptions-instans med konstruktorn och LoadFormat‑parameter
                HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);

                // Ställ in några egenskaper för HtmlLoadOptions
                loadOptions.AutoFitColsAndRows = true;
                loadOptions.SupportDivTag = true;
                loadOptions.DeleteRedundantSpaces = true;

                // Skapa en arbetsbok med laddningsalternativen
                Workbook workbook = new Workbook("input.html", loadOptions);

                // Åtkomst till det första kalkylbladet
                Worksheet worksheet = workbook.Worksheets[0];

                // Visa viss information om den laddade HTML‑en
                Console.WriteLine("HTML loaded successfully with LoadFormat.Html");
                Console.WriteLine($"Worksheet name: {worksheet.Name}");
                Console.WriteLine($"Cells count: {worksheet.Cells.MaxDataRow + 1} rows x {worksheet.Cells.MaxDataColumn + 1} columns");

                // Spara arbetsboken
                workbook.Save("HtmlLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading HTML file: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [LoadFormat](../../loadformat/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


