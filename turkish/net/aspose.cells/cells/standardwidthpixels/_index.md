---
title: "Cells.StandardWidthPixels"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Çalışma sayfasındaki varsayılan sütun genişliğini piksel biriminde alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/cells/standardwidthpixels/
---
## Cells.StandardWidthPixels property

Çalışma sayfasındaki varsayılan sütun genişliğini, piksel biriminde alır veya ayarlar.

```csharp
public int StandardWidthPixels { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardWidthPixelsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Standart genişliği piksel cinsinden ayarlayın ve alın
            cells.StandardWidthPixels = 104;
            Console.WriteLine("Standard Width in Pixels: " + cells.StandardWidthPixels);

            // Standart genişliği karakter cinsinden ayarlayın ve alın
            cells.StandardWidth = 12.375;
            Console.WriteLine("Standard Width in Characters: " + cells.StandardWidth);

            // Standart yüksekliği nokta cinsinden ayarlayın ve alın
            cells.StandardHeight = 14.25;
            Console.WriteLine("Standard Height in Points: " + cells.StandardHeight);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


