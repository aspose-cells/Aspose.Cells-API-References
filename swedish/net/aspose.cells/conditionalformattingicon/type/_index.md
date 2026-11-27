---
title: "ConditionalFormattingIcon.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ConditionalFormattingIcon-egenskapen. Hämtar och anger ikonuppsättningstypen"
type: docs
url: /sv/net/aspose.cells/conditionalformattingicon/type/
---
## ConditionalFormattingIcon.Type property

Hämtar och anger ikonuppsättningstypen.

```csharp
public IconSetType Type { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingIconPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Lägg till villkorsstyrd formatering med ikonuppsättning
            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            int index = cfs.Add();
            FormatConditionCollection fc = cfs[index];
            fc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 2, EndColumn = 0 });
            
            int conditionIndex = fc.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fc[conditionIndex];
            condition.IconSet.Type = IconSetType.Symbols3;
            
            // Tillämpa formatering och beräkna
            workbook.CalculateFormula();

            // Hämta formateringsresultat och demonstrera Type-egenskapen
            Cell cell = worksheet.Cells["A2"];
            ConditionalFormattingResult formattingResult = cell.GetConditionalFormattingResult();
            
            Console.WriteLine("Icon Set Type: " + formattingResult.ConditionalFormattingIcon.Type);
            Console.WriteLine("Icon Index: " + formattingResult.ConditionalFormattingIcon.Index);
        }
    }
}
```

### Se även

* enum [IconSetType](../../iconsettype/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


