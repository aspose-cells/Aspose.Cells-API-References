---
title: "MsoFillFormat.ForeColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoFillFormat özelliği. Dolgu ön rengini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/msofillformat/forecolor/
---
## MsoFillFormat.ForeColor property

Doldurma ön rengini alır ve ayarlar.

```csharp
public Color ForeColor { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatPropertyForeColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gerekli tüm parametrelerle bir dikdörtgen şekil ekle
            var rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 150, 200);

            // Dolgu formatını al
            MsoFillFormat fillFormat = rectangle.FillFormat;

            // ForeColor özelliğini ayarla ve göster
            fillFormat.ForeColor = System.Drawing.Color.Red;
            Console.WriteLine("ForeColor set to: " + fillFormat.ForeColor);

            // ForeColor'ı değiştir
            fillFormat.ForeColor = System.Drawing.Color.FromArgb(0, 128, 255);
            Console.WriteLine("ForeColor changed to: " + fillFormat.ForeColor);

            // Çalışma kitabını kaydedin
            workbook.Save("MsoFillFormatForeColorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


