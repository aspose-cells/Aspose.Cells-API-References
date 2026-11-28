---
title: "Shape.InputRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Belirtilen combo kutusunu doldurmak için kullanılan çalışma sayfası aralığını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/inputrange/
---
## Shape.InputRange property

Belirtilen combo kutusunu doldurmak için kullanılan çalışma sayfası aralığını alır veya ayarlar.

```csharp
public string InputRange { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyInputRangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Value 1");
            worksheet.Cells["A2"].PutValue("Value 2");
            worksheet.Cells["A3"].PutValue("Value 3");
            worksheet.Cells["A4"].PutValue("Value 4");
            worksheet.Cells["A5"].PutValue("Value 5");

            // Bir şekil (dikdörtgen) ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Şekil için giriş aralığını ayarla
            shape.InputRange = "$A$1:$A$5";

            // Gerekirse giriş aralığını kontrol et ve değiştir
            if (shape.InputRange.Equals("$A$1:$A$5"))
            {
                shape.InputRange = "$B$1:$B$5";
                Console.WriteLine("Input range changed to: " + shape.InputRange);
            }
            else
            {
                Console.WriteLine("Current input range: " + shape.InputRange);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


