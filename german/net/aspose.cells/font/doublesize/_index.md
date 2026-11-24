---
title: "Font.DoubleSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Font-Eigenschaft. Gibt die doppelte Größe der Schrift zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells/font/doublesize/
---
## Font.DoubleSize property

Ruft die doppelte Größe der Schrift ab und legt sie fest.

```csharp
public double DoubleSize { get; set; }
```

### Beispiele

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

### Siehe auch

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


