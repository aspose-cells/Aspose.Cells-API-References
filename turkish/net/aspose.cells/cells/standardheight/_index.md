---
title: "Cells.StandardHeight"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Bu çalışma sayfasındaki varsayılan satır yüksekliğini puan biriminde alır veya ayarlar."
type: docs
url: /tr/net/aspose.cells/cells/standardheight/
---
## Cells.StandardHeight property

Bu çalışma sayfasındaki varsayılan satır yüksekliğini, nokta biriminde alır veya ayarlar.

```csharp
public double StandardHeight { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardHeightDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Standart yüksekliği al ve göster
            double standardHeight = worksheet.Cells.StandardHeight;
            Console.WriteLine("Standard Height: " + standardHeight);
            
            // Yeni bir standart yükseklik ayarla
            worksheet.Cells.StandardHeight = 20;
            Console.WriteLine("New Standard Height: " + worksheet.Cells.StandardHeight);
            
            // Çalışma kitabını kaydedin
            workbook.Save("StandardHeightDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


