---
title: "Spinner.IncrementalChange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Spinner özelliği. Kaydırma çubuğu veya spinner'ın bir satır kaydırma ile artırıldığı miktarı alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/spinner/incrementalchange/
---
## Spinner.IncrementalChange property

Kaydırma çubuğu veya döndürme düğmesinin bir satır kaydırma ile artırıldığı miktarı alır veya ayarlar.

```csharp
public int IncrementalChange { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyIncrementalChangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir spinner denetimi oluştur
            Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 100);

            // Spinner özelliklerini ayarla
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.CurrentValue = 50;
            spinner.IncrementalChange = 5; // Demonstrate IncrementalChange property

            // IncrementalChange değerini doğrula ve çıktı ver
            Console.WriteLine("Spinner IncrementalChange: " + spinner.IncrementalChange);

            // Değiştir ve tekrar doğrula
            spinner.IncrementalChange = 10;
            Console.WriteLine("Modified IncrementalChange: " + spinner.IncrementalChange);

            // Çalışma kitabını kaydedin
            workbook.Save("SpinnerIncrementalChangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


