---
title: "Spinner.Shadow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Spinner özelliği. Şeklin 3D gölgelendirmeye sahip olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/spinner/shadow/
---
## Spinner.Shadow property

Şeklin 3B gölgelendirmeye sahip olup olmadığını gösterir.

```csharp
public bool Shadow { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyShadowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir spinner ekle
            Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 30);

            // Spinner özelliklerini ayarla
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;
            spinner.CurrentValue = 50;

            // Shadow özelliğini göster
            spinner.Shadow = true; // Enable 3D shadow effect
            Console.WriteLine("Spinner shadow enabled: " + spinner.Shadow);

            // Çalışma kitabını kaydedin
            workbook.Save("SpinnerShadowDemo.xlsx");

            // Gölge özelliğini doğrulamak için kaydedilmiş çalışma kitabını yükleyin
            Workbook verifyWorkbook = new Workbook("SpinnerShadowDemo.xlsx");
            Spinner verifySpinner = (Spinner)verifyWorkbook.Worksheets[0].Shapes[0];
            Console.WriteLine("Verified spinner shadow: " + verifySpinner.Shadow);
        }
    }
}
```

### Ayrıca Bakınız

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


