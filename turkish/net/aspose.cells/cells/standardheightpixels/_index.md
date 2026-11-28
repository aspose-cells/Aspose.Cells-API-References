---
title: "Cells.StandardHeightPixels"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Bu çalışma sayfasındaki varsayılan satır yüksekliğini piksel biriminde alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/cells/standardheightpixels/
---
## Cells.StandardHeightPixels property

Bu çalışma sayfasındaki varsayılan satır yüksekliğini, piksel biriminde alır veya ayarlar.

```csharp
public int StandardHeightPixels { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardHeightPixelsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Hücrelere bazı veriler ayarla
            cells["A1"].PutValue("Sample Data");
            cells["B2"].PutValue(123);
            cells["C3"].PutValue(DateTime.Now);

            // Standart yüksekliği piksel cinsinden al
            int standardHeight = cells.StandardHeightPixels;
            Console.WriteLine("Standard row height in pixels: " + standardHeight);

            // Satır yüksekliklerini göster (standart yükseklik ile eşleşmeli)
            for (int i = 0; i < 5; i++)
            {
                int rowHeight = cells.GetRowHeightPixel(i);
                Console.WriteLine($"Row {i} height: {rowHeight}px");
                Console.WriteLine($"Matches standard: {rowHeight == standardHeight}");
            }

            // Standart yüksekliği değiştir ve doğrula
            cells.StandardHeight = 20; // Set in points
            int newStandardHeight = cells.StandardHeightPixels;
            Console.WriteLine("\nNew standard height in pixels: " + newStandardHeight);

            // Tüm satırların artık yeni yüksekliğe sahip olduğunu doğrula
            for (int i = 0; i < 5; i++)
            {
                int rowHeight = cells.GetRowHeightPixel(i);
                Console.WriteLine($"Row {i} height: {rowHeight}px");
                Console.WriteLine($"Matches new standard: {rowHeight == newStandardHeight}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


