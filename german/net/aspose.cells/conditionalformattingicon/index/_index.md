---
title: "ConditionalFormattingIcon.Index"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ConditionalFormattingIcon-Eigenschaft. Liest und schreibt den Index des Symbols im Symbolset"
type: docs
url: /de/net/aspose.cells/conditionalformattingicon/index/
---
## ConditionalFormattingIcon.Index property

Liefert und setzt den Index des Symbols im Symbolset.

```csharp
public int Index { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingIconPropertyIndexDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);

            // Fügen Sie eine bedingte Formatierung für das Symbolset hinzu
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.IconSet);
            
            // Icon-Set-Eigenschaften festlegen
            FormatCondition condition = fcc[0];
            condition.IconSet.Type = IconSetType.Arrows3;
            ConditionalFormattingIconCollection icons = condition.IconSet.CfIcons;

            // Den Index jedes Symbols anzeigen
            Console.WriteLine("Icon Indexes:");
            for (int i = 0; i < icons.Count; i++)
            {
                Console.WriteLine($"Icon {i}: Index = {icons[i].Index}");
            }

            // Index-Eigenschaft ändern und anzeigen
            icons[1].Index = 2;
            Console.WriteLine($"Modified Icon 1 Index: {icons[1].Index}");
        }
    }
}
```

### Siehe auch

* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


