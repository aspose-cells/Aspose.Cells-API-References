---
title: "Cell.StringValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell‑egenskap. Hämtar strängvärdet som finns i cellen. Om cellens typ är sträng returneras själva strängvärdet. För andra celltyper returneras det formaterade strängvärdet som formaterats med cellens angivna stil. Det formaterade cellvärdet är detsamma som du kan få från Excel när du kopierar en cell som text, till exempel när du kopierar cellen till en textredigerare eller exporterar till CSV"
type: docs
url: /sv/net/aspose.cells/cell/stringvalue/
---
## Cell.StringValue property

Hämtar strängvärdet som finns i cellen. Om cellens typ är sträng returneras själva strängvärdet. För andra celltyper returneras det formaterade strängvärdet (formaterat med den angivna stilen för den här cellen). Det formaterade cellvärdet är detsamma som vad du kan få i Excel när du kopierar en cell som text (t.ex. kopierar cellen till en textredigerare eller exporterar till CSV).

```csharp
public string StringValue { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyStringValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ange några värden
            cells["A1"].PutValue("Hello");
            cells["A2"].PutValue(123);
            cells["A3"].PutValue(DateTime.Now);
            cells["A4"].Formula = "=A1&A2";

            // Beräkna formler
            workbook.CalculateFormula();

            // Demonstrera egenskapen StringValue
            Console.WriteLine("A1 StringValue: " + cells["A1"].StringValue);
            Console.WriteLine("A2 StringValue: " + cells["A2"].StringValue);
            Console.WriteLine("A3 StringValue: " + cells["A3"].StringValue);
            Console.WriteLine("A4 StringValue: " + cells["A4"].StringValue);

            // Visa felvärdesfall
            Cell errorCell = cells["B1"];
            errorCell.Formula = "=1/0";
            workbook.CalculateFormula();
            Console.WriteLine("B1 (Error) StringValue: " + errorCell.StringValue);
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


