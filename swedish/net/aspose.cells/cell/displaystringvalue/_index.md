---
title: "Cell.DisplayStringValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-egenskap. Hämtar det formaterade strängvärdet för denna cell enligt cellens visningsstil"
type: docs
url: /sv/net/aspose.cells/cell/displaystringvalue/
---
## Cell.DisplayStringValue property

Hämtar det formaterade strängvärdet för den här cellen enligt cellens visningsstil.

```csharp
public string DisplayStringValue { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyDisplayStringValueDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cell cell = sheet.Cells[0, 0];
            
            // Första exemplet
            Style style = cell.GetStyle();
            style.Custom = "# ##/##\\\"";
            cell.SetStyle(style);
            cell.PutValue(3);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: 3"
            
            // Andra exemplet
            style.Custom = "\"a\"#\"b\" \"c\"##\"d\"/\"e\"##";
            cell.SetStyle(style);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a3
            
            // Tredje exemplet
            style.Custom = "\"a\"#\"b\" \"c\"##\"d\"/\"e\"##\"f\"";
            cell.SetStyle(style);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a3f
            
            // Fjärde exemplet med decimalt värde
            cell.PutValue(1.234);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a1b c11d/e47f
            
            // Femte exemplet med modifierat format
            style.Custom = "\"a\"#\"b\"\"c\"##\"d\"/\"e\"##\"f\"";
            cell.SetStyle(style);
            cell.PutValue(3);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a3f
            
            // Sjätte exemplet med decimalt värde
            cell.PutValue(1.234);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a1bc11d/e47f
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


