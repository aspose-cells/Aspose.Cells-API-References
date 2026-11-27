---
title: "ConditionalFormattingIcon.Index"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ConditionalFormattingIcon-egenskapen. Hämtar och anger ikonens index i ikonuppsättningen"
type: docs
url: /sv/net/aspose.cells/conditionalformattingicon/index/
---
## ConditionalFormattingIcon.Index property

Hämtar och anger ikonens index i ikonuppsättningen.

```csharp
public int Index { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingIconPropertyIndexDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);

            // Lägg till villkorsformatering med ikonset
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.IconSet);
            
            // Ställ in egenskaper för ikonsats
            FormatCondition condition = fcc[0];
            condition.IconSet.Type = IconSetType.Arrows3;
            ConditionalFormattingIconCollection icons = condition.IconSet.CfIcons;

            // Visa index för varje ikon
            Console.WriteLine("Icon Indexes:");
            for (int i = 0; i < icons.Count; i++)
            {
                Console.WriteLine($"Icon {i}: Index = {icons[i].Index}");
            }

            // Ändra och visa indexegenskapen
            icons[1].Index = 2;
            Console.WriteLine($"Modified Icon 1 Index: {icons[1].Index}");
        }
    }
}
```

### Se även

* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


