---
title: "Spinner.Max"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Spinner özelliği. Kaydırma çubuğu veya spinner aralığının maksimum değerini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/spinner/max/
---
## Spinner.Max property

Kaydırma çubuğu veya döndürme düğmesi aralığının maksimum değerini alır veya ayarlar.

```csharp
public int Max { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyMaxDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            Aspose.Cells.Drawing.Spinner spinner = sheet.Shapes.AddSpinner(1, 1, 0, 0, 100, 100);
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;

            Console.WriteLine($"Spinner Max Value: {spinner.Max}");
        }
    }
}
```

### Ayrıca Bakınız

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


