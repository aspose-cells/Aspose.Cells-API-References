---
title: "UnionRange.Value"
second_title: "Aspose.Cells için .NET API Referansı"
description: "UnionRange özelliği. Aralığın değerlerini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/unionrange/value/
---
## UnionRange.Value property

Aralığın değerlerini alır ve ayarlar.

```csharp
public object Value { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class UnionRangePropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Doğru API'yi kullanarak bir birleşim aralığı oluştur.
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:B2,D1:E2", 0);
            
            // Tüm birleşim aralığı için değeri ayarla.
            unionRange.Value = "Test Value";
            
            // Stil oluştur ve uygula
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            unionRange.ApplyStyle(style, new StyleFlag { All = true });
            
            // Çalışma kitabını kaydedin
            workbook.Save("UnionRangeValueDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


