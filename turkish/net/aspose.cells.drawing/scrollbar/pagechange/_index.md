---
title: "ScrollBar.PageChange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ScrollBar özelliği. Sayfa değişimini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/scrollbar/pagechange/
---
## ScrollBar.PageChange property

Sayfa değişimini alır veya ayarlar

```csharp
public int PageChange { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyPageChangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir kaydırma çubuğu ekleyin
            ScrollBar scrollBar = worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Kaydırma çubuğu özelliklerini ayarlayın
            scrollBar.Min = 0;
            scrollBar.Max = 100;
            scrollBar.CurrentValue = 50;
            scrollBar.IncrementalChange = 1;
            scrollBar.PageChange = 10; // Demonstrate PageChange property
            scrollBar.LinkedCell = "A1";

            // Çalışma kitabını kaydedin
            workbook.Save("ScrollBarPropertyPageChangeDemo.xlsx");

            // Kaydedilmiş çalışma kitabını yükleyerek özellikleri doğrulayın
            Workbook verifyWorkbook = new Workbook("ScrollBarPropertyPageChangeDemo.xlsx");
            ScrollBar verifyScrollBar = (ScrollBar)verifyWorkbook.Worksheets[0].Shapes[0];

            // PageChange özelliği değerini çıktılayarak doğru şekilde kaydedildi/kaydedildiğini göster
            Console.WriteLine("ScrollBar PageChange value: " + verifyScrollBar.PageChange);
        }
    }
}
```

### Ayrıca Bakınız

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


