---
title: "UnionRange.HasRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà UnionRange. Indica se questo ha un intervallo"
type: docs
url: /it/net/aspose.cells/unionrange/hasrange/
---
## UnionRange.HasRange property

Indica se questo ha un intervallo.

```csharp
public bool HasRange { get; }
```

### Esempi

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
            
            // Crea un intervallo di unione usando l'API corretta
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A5,B1:B5", 0);
            
            // Verifica se l'intervallo di unione ha intervalli validi
            Console.WriteLine("UnionRange has ranges: " + unionRange.HasRange);
            
            // Imposta valore e stile solo se l'intervallo è valido
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

### Vedi anche

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


