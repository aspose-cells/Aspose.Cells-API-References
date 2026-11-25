---
title: "Style.ForegroundColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Ottiene o imposta il colore di primo piano di uno stile"
type: docs
url: /it/net/aspose.cells/style/foregroundcolor/
---
## Style.ForegroundColor property

Ottiene o imposta il colore di primo piano di uno stile.

```csharp
public Color ForegroundColor { get; set; }
```

### Osservazioni

Significa che non è impostato alcun colore se viene restituito Color.Empty.

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyForegroundColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            Style style = workbook.CreateStyle();
            style.ForegroundColor = Color.Green;
            style.Pattern = BackgroundType.Solid;
            
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            Console.WriteLine("ForegroundColor set to: " + style.ForegroundColor);
            
            workbook.Save("ForegroundColorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


