---
title: "Style.IsGradient"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Hücre gölgelendirmenin bir degrade desen olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/style/isgradient/
---
## Style.IsGradient property

Hücre gölgelendirmenin bir degrade deseni olup olmadığını gösterir.

```csharp
public bool IsGradient { get; set; }
```

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyIsGradientDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir stil oluştur
            Style style = workbook.CreateStyle();
            
            // Degrade arka planı ayarla
            style.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 1);
            
            // Stili bir hücreye uygula
            worksheet.Cells["A1"].SetStyle(style);
            
            // Stilin degrade içerip içermediğini kontrol et
            bool isGradient = worksheet.Cells["A1"].GetStyle().IsGradient;
            
            // Sonucu çıktı olarak ver
            Console.WriteLine("Cell A1 style has gradient: " + isGradient);
            
            // Çalışma kitabını kaydedin
            workbook.Save("GradientStyleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


