---
title: "AbstractTextLoadOptions.KeepPrecision"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractTextLoadOptions-egenskap. Anger huruvida en strängvärde inte ska parsas om längden är 15"
type: docs
url: /sv/net/aspose.cells/abstracttextloadoptions/keepprecision/
---
## AbstractTextLoadOptions.KeepPrecision property

Indikerar om en strängvärde inte ska parsas om längden är 15.

```csharp
public bool KeepPrecision { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyKeepPrecisionDemo
    {
        public static void Run()
        {
            // Skapa HTML-inläsningsalternativ och sätt KeepPrecision till true
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.KeepPrecision = true;

            // Läs in arbetsboken med alternativen
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Visa att precisionen bibehålls (t.ex. numeriska värden med många decimaler)
            Cell cell = worksheet.Cells["A1"];
            Console.WriteLine("Value with precision: " + cell.Value);

            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


