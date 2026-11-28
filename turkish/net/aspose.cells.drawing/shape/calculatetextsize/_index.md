---
title: "Shape.CalculateTextSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape yöntemi. Metin alanını yeniden hesapla"
type: docs
url: /tr/net/aspose.cells.drawing/shape/calculatetextsize/
---
## Shape.CalculateTextSize method

Metin alanını yeniden hesapla

```csharp
public int[] CalculateTextSize()
```

### Dönüş Değeri

Metnin Boyutu bir dizi içinde (genişlik ve yükseklik).

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodCalculateTextSizeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine örnek bir metin ekle
            worksheet.Cells["A1"].PutValue("Sample Text for Size Calculation");

            // Tüm gerekli parametrelerle bir dikdörtgen şekli oluştur
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            // Şekle metin ayarla
            shape.Text = "This is a test string to calculate text size";

            // Metin boyutunu hesapla
            int[] size = shape.CalculateTextSize();

            // Sonuçları çıktı olarak ver.
            Console.WriteLine($"Calculated text size - Width: {size[0]}, Height: {size[1]}");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


