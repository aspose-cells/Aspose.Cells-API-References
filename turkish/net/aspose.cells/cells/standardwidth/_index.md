---
title: "Cells.StandardWidth"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Çalışma sayfasındaki varsayılan sütun genişliğini karakter biriminde alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/cells/standardwidth/
---
## Cells.StandardWidth property

Çalışma sayfasındaki varsayılan sütun genişliğini, karakter biriminde alır veya ayarlar.

```csharp
public double StandardWidth { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardWidthDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Sütunlar için standart genişliği ayarla
            cells.StandardWidth = 18.25;

            // İlk sütunun standart ve gerçek genişliğini göster
            Console.WriteLine("Standard Width: " + cells.StandardWidth);
            Console.WriteLine("Column 0 Width: " + cells.GetColumnWidth(0));

            // Standart genişliğin uygulandığını doğrula (yaklaşık olarak)
            if (Math.Abs(cells.GetColumnWidth(0) - cells.StandardWidth) > 1.0)
            {
                Console.WriteLine("Warning: Column width differs significantly from standard width");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


