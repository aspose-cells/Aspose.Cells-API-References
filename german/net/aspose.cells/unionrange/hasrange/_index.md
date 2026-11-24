---
title: "UnionRange.HasRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "UnionRange-Eigenschaft. Gibt an, ob dies einen Bereich hat"
type: docs
url: /de/net/aspose.cells/unionrange/hasrange/
---
## UnionRange.HasRange property

Gibt an, ob dies einen Bereich hat.

```csharp
public bool HasRange { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class UnionRangePropertyHasRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle einen Vereinigungsbereich mit der richtigen API
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A5,B1:B5", 0);
            
            // Prüfe, ob der UnionRange gültige Bereiche hat
            Console.WriteLine("UnionRange has ranges: " + unionRange.HasRange);
            
            // Setze Wert und Stil nur, wenn der Bereich gültig ist
            if (unionRange.HasRange)
            {
                unionRange.Value = "Test Value";
                
                Style style = workbook.CreateStyle();
                style.Pattern = BackgroundType.Solid;
                style.ForegroundColor = System.Drawing.Color.LightBlue;
                unionRange.ApplyStyle(style, new StyleFlag { All = true });
            }
            
            workbook.Save("UnionRangeHasRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


