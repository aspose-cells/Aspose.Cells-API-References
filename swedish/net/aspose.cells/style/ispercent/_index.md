---
title: "Style.IsPercent"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style‑egenskap. Anger om talformatet är ett procentformat"
type: docs
url: /sv/net/aspose.cells/style/ispercent/
---
## Style.IsPercent property

Anger om talformatet är ett procentformat.

```csharp
public bool IsPercent { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StylePropertyIsPercentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till cell A1 och ange dess värde
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(0.5);
            
            // Hämta stil för cellen
            Style style = cell.GetStyle();
            
            // Visa aktuellt IsPercent‑värde
            Console.WriteLine("Current IsPercent value: " + style.IsPercent);
            
            // Ställ in talformat till procent (detta kommer automatiskt att sätta IsPercent till true)
            style.Number = 10; // 10 is the built-in percentage format in Excel
            
            // Tillämpa stilen på cellen
            cell.SetStyle(style);
            
            // Verifiera att IsPercent nu är true
            Console.WriteLine("After setting percentage format, IsPercent value: " + style.IsPercent);
            
            // Skapa en annan cell med annat format
            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue(0.75);
            Style style2 = cell2.GetStyle();
            style2.Number = 3; // 3 is the built-in number format (not percentage)
            cell2.SetStyle(style2);
            
            // Verifiera att IsPercent är false för icke‑procentformat
            Console.WriteLine("For non-percentage format, IsPercent value: " + style2.IsPercent);
            
            // Spara arbetsboken
            workbook.Save("StylePropertyIsPercentDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


