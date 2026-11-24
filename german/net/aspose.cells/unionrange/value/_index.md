---
title: "UnionRange.Value"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "UnionRange-Eigenschaft. Ruft die Werte des Bereichs ab und legt sie fest"
type: docs
url: /de/net/aspose.cells/unionrange/value/
---
## UnionRange.Value property

Liest und setzt die Werte des Bereichs.

```csharp
public object Value { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class UnionRangePropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle einen Vereinigungsbereich mit der richtigen API
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:B2,D1:E2", 0);
            
            // Setze den Wert für den gesamten Vereinigungsbereich
            unionRange.Value = "Test Value";
            
            // Erstellen und Anwenden eines Stils
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            unionRange.ApplyStyle(style, new StyleFlag { All = true });
            
            // Speichere die Arbeitsmappe
            workbook.Save("UnionRangeValueDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


