---
title: "UnionRange.HasRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "UnionRange özelliği. Bunun bir aralığı olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/unionrange/hasrange/
---
## UnionRange.HasRange property

Bu öğenin aralığa sahip olup olmadığını gösterir.

```csharp
public bool HasRange { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class UnionRangePropertyHasRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Doğru API'yi kullanarak bir birleşim aralığı oluştur.
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A5,B1:B5", 0);
            
            // Birleşik aralığın geçerli aralıkları olup olmadığını kontrol edin
            Console.WriteLine("UnionRange has ranges: " + unionRange.HasRange);
            
            // Aralık geçerli ise yalnızca değeri ve stili ayarla
            if (unionRange.HasRange)
            {
                unionRange.Value = "Test Value";
                
                Style style = workbook.CreateStyle();
                style.Pattern = BackgroundType.Solid;
                style.ForegroundColor = System.Drawing.Color.LightBlue;
                unionRange.ApplyStyle(style, new StyleFlag { All = true });
            }
            
            workbook.Save("UnionRangeHasRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


