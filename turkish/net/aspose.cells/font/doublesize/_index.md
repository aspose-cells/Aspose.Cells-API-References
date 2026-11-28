---
title: "Font.DoubleSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Font özelliği. Yazı tipinin çift boyutunu alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/font/doublesize/
---
## Font.DoubleSize property

Yazı tipinin çift boyutunu alır ve ayarlar.

```csharp
public double DoubleSize { get; set; }
```

### Örnekler

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

### Ayrıca Bakınız

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


