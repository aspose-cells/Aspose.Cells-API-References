---
title: "Cells.Style"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Hämtar och anger standardstilen för arbetsbladet"
type: docs
url: /sv/net/aspose.cells/cells/style/
---
## Cells.Style property

Hämtar och anger standardstilen för kalkylbladet.

```csharp
public Style Style { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ange ett värde i cell A1
            Cell cell = cells["A1"];
            cell.PutValue(43368); // This represents the date 2018-09-25

            // Hämta standardstilen och ändra dess format
            Style style = cells.Style;
            style.CultureCustom = "yyyymmdd!y";
            
            // Applicera den modifierade stilen på cellen
            cell.SetStyle(style);

            // Visa det formaterade strängvärdet
            Console.WriteLine("Formatted value: " + cell.StringValue);
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


