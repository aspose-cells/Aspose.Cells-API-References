---
title: "Spinner.IsHorizontal"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Spinner özelliği. Bunun yatay bir kaydırma çubuğu olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/spinner/ishorizontal/
---
## Spinner.IsHorizontal property

Bunun yatay bir kaydırma çubuğu olup olmadığını gösterir.

```csharp
public bool IsHorizontal { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class SpinnerPropertyIsHorizontalDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Çalışma sayfasına bir spinner şekli ekleyin
                Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 30);
                
                // Spinner özelliklerini ayarla
                spinner.Min = 0;
                spinner.Max = 100;
                spinner.IncrementalChange = 5;
                spinner.CurrentValue = 50;
                
                // IsHorizontal özelliğini gösterin (okuma ve yazma)
                Console.WriteLine("Initial IsHorizontal value: " + spinner.IsHorizontal);
                
                // Yönelimi değiştirin
                spinner.IsHorizontal = !spinner.IsHorizontal;
                Console.WriteLine("Modified IsHorizontal value: " + spinner.IsHorizontal);
                
                // Çalışma kitabını kaydedin
                workbook.Save("SpinnerIsHorizontalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


