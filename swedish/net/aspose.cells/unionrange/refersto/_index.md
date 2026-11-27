---
title: "UnionRange.RefersTo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "UnionRange‑egenskap. Hämtar de områden som den refererar till"
type: docs
url: /sv/net/aspose.cells/unionrange/refersto/
---
## UnionRange.RefersTo property

Hämtar vad området refererar till.

```csharp
public string RefersTo { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyRefersToDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i lite data
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(800);

            // Skapa ett namngivet område
            Aspose.Cells.Range namedRange = worksheet.Cells.CreateRange("B2:B3");
            namedRange.Name = "ProductPrices";

            // Skapa ett unionområde som inkluderar vårt namngivna område
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B3").UnionRanges(new Aspose.Cells.Range[] { namedRange });

            // Visa RefersTo‑egenskapen för unionområdet
            Console.WriteLine("UnionRange RefersTo: " + unionRange.RefersTo);

            // Skapa ett annat område och visa dess RefersTo
            Aspose.Cells.Range singleRange = worksheet.Cells.CreateRange("C1:D3");
            Console.WriteLine("Single Range RefersTo: " + singleRange.RefersTo);

            // Demonstrera hur man använder RefersTo för att identifiera områdessammansättningen
            Console.WriteLine("Does union range contain named range? " + 
                unionRange.RefersTo.Contains("ProductPrices"));

            // Visa hur RefersTo förändras när områden ändras
            Aspose.Cells.Range newRange = worksheet.Cells.CreateRange("A1:C3");
            UnionRange modifiedUnion = newRange.UnionRanges(new Aspose.Cells.Range[] { namedRange });
            Console.WriteLine("Modified UnionRange RefersTo: " + modifiedUnion.RefersTo);

            // Spara arbetsboken
            workbook.Save("UnionRangeRefersToDemo.xlsx");
        }
    }
}
```

### Se även

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


