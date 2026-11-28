---
title: "Range.EntireColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range özelliği. Belirtilen aralığı içeren tüm sütunu veya sütunları temsil eden bir Range nesnesi döndürür."
type: docs
url: /tr/net/aspose.cells/range/entirecolumn/
---
## Range.EntireColumn property

Belirtilen aralığı içeren tüm sütunu (veya sütunları) temsil eden bir Range nesnesi alır.

```csharp
public Range EntireColumn { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyEntireColumnDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // C1 hücresinde (satır 0, sütun 2) başlayan bir aralık oluşturun
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 2, 1, 1);
            
            // Aralığı içeren tüm sütunu alın (sütun C)
            Aspose.Cells.Range entireColumn = range.EntireColumn;
            
            // Tüm sütuna biçimlendirme uygulayın
            Style style = entireColumn[0, 0].GetStyle();
            style.Custom = "##0%";
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.NumberFormat = true;
            entireColumn.ApplyStyle(style, styleFlag);
            
            // Çalışma kitabını kaydedin
            workbook.Save("EntireColumnDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


