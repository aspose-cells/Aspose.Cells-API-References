---
title: "UnionRange.Value"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà UnionRange. Ottiene e imposta i valori dell'intervallo"
type: docs
url: /it/net/aspose.cells/unionrange/value/
---
## UnionRange.Value property

Ottiene e imposta i valori dell'intervallo.

```csharp
public object Value { get; set; }
```

### Esempi

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
            
            // Crea un intervallo di unione usando l'API corretta
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:B2,D1:E2", 0);
            
            // Imposta il valore per l'intero intervallo di unione
            unionRange.Value = "Test Value";
            
            // Crea e applica lo stile
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            unionRange.ApplyStyle(style, new StyleFlag { All = true });
            
            // Salva la cartella di lavoro
            workbook.Save("UnionRangeValueDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


