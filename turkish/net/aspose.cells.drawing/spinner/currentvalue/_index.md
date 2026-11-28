---
title: "Spinner.CurrentValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Spinner özelliği. Mevcut değeri alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/spinner/currentvalue/
---
## Spinner.CurrentValue property

Geçerli değeri alır veya ayarlar.

```csharp
public int CurrentValue { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyCurrentValueDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir spinner denetimi ekleyin
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Spinner, 1, 1, 0, 0, 20, 20);
            Spinner spinner = (Spinner)shape;

            // Spinner özelliklerini ayarla
            spinner.LinkedCell = "A1";
            spinner.Min = 1;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;
            spinner.CurrentValue = 10; // Using CurrentValue property directly

            // Mevcut değeri doğrulayın ve çıktı verin
            Console.WriteLine("Spinner CurrentValue: " + spinner.CurrentValue);

            // Çalışma kitabını kaydedin
            workbook.Save("SpinnerDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


