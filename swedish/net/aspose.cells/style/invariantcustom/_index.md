---
title: "Style.InvariantCustom"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style‑egenskap. Hämtar det kulturoberoende mönstersträngen för talformat. Om inget talformat har angetts för detta objekt returneras null. Om talformatet är inbyggt returneras mönstersträngen som motsvarar det inbyggda talet."
type: docs
url: /sv/net/aspose.cells/style/invariantcustom/
---
## Style.InvariantCustom property

Hämtar det kulturoberoende mönsterssträngen för talformat. Om inget talformat har satts för detta objekt returneras null. Om talformatet är inbyggt returneras mönsterssträngen som motsvarar det inbyggda talet.

```csharp
public string InvariantCustom { get; }
```

### Anmärkningar

För inbyggda talformat är det returnerade mönsterinnehållet fortfarande kulturberoende, till exempel returnerar vissa språk "m/d/y" och andra språk "d/m/y". Skillnaden från [`CultureCustom`](../culturecustom/) är (det är också vad kulturoberoende betyder): formatspecifierare och avgränsare behålls som standard, så '/' alltid används som datum‑tid‑avgränsare och "y" alltid används som "år"‑delen oavsett vilken annan specialtecken som används för den specifika språkinställningen.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyInvariantCustomDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.Germany;
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            Style style = cell.GetStyle();
            
            // Ange datumformat och värde
            style.Number = 14; // Date format
            style.Custom = "dd/MM/yyyy"; // Set custom format which affects both CultureCustom and InvariantCustom
            cell.PutValue(new DateTime(2019, 10, 12));
            cell.SetStyle(style);

            // Skriv ut resultat
            Console.WriteLine("Formatted value: " + cell.StringValue);
            Console.WriteLine("CultureCustom: " + style.CultureCustom);
            Console.WriteLine("InvariantCustom: " + style.InvariantCustom);
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


