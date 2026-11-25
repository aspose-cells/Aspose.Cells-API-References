---
title: "Font.DoubleSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Font. Ottiene e imposta la dimensione doppia del carattere"
type: docs
url: /it/net/aspose.cells/font/doublesize/
---
## Font.DoubleSize property

Ottiene e imposta la dimensione doppia del carattere.

```csharp
public double DoubleSize { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyDoubleSizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Style style = cell.GetStyle();
            style.Font.DoubleSize = 10.5;
            cell.SetStyle(style);
            
            Console.WriteLine("Font DoubleSize set to: " + cell.GetStyle().Font.DoubleSize);
        }
    }
}
```

### Vedi anche

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


