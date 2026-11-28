---
title: "Spinner.Min"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Spinner özelliği. Kaydırma çubuğu veya spinner aralığının minimum değerini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/spinner/min/
---
## Spinner.Min property

Kaydırma çubuğu veya döndürme düğmesi aralığının minimum değerini alır veya ayarlar.

```csharp
public int Min { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyMinDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Uygun boyutlarda bir spinner denetimi ekleyin
            Spinner spinner = worksheet.Shapes.AddSpinner(1, 1, 1, 1, 100, 20);

            // Min dahil olmak üzere spinner özelliklerini ayarlayın
            spinner.Min = 10;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;
            spinner.CurrentValue = 15;

            // Min özelliğini doğrulayın ve çıktı verin
            Console.WriteLine("Spinner Min Value: " + spinner.Min);

            // Çalışma kitabını kaydedin
            workbook.Save("SpinnerPropertyMinDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


