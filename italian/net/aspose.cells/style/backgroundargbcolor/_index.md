---
title: "Style.BackgroundArgbColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Ottiene e imposta il colore di sfondo con un valore ARGB a 32 bit"
type: docs
url: /it/net/aspose.cells/style/backgroundargbcolor/
---
## Style.BackgroundArgbColor property

Ottiene e imposta il colore di sfondo con un valore ARGB a 32 bit.

```csharp
public int BackgroundArgbColor { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyBackgroundArgbColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Style style = cell.GetStyle();
            style.BackgroundArgbColor = Color.Yellow.ToArgb();
            style.Pattern = BackgroundType.Solid;
            
            cell.SetStyle(style);
            cell.PutValue("Sample Text with Yellow Background");
            
            workbook.Save("BackgroundArgbColorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


