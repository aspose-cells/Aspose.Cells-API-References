---
title: "Fill.Equals"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Fill yöntemi. /"
type: docs
url: /tr/net/aspose.cells.drawing/fill/equals/
---
## Fill.Equals method

/

```csharp
public override bool Equals(object obj)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | Object |  |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class FillMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Çalışma sayfasına bir dikdörtgen şekli ekle
                Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 0, 0, 100, 150);

                // Şekilden FillFormat nesnesini al
                FillFormat fillFormat1 = rectangle.Fill;

                // İkinci bir FillFormat nesnesi elde etmek için başka bir şekil oluştur
                Shape oval = worksheet.Shapes.AddOval(3, 0, 0, 0, 100, 150);
                FillFormat fillFormat2 = oval.Fill;

                // İki FillFormat nesnesini karşılaştırmak için Equals metodunu çağır
                bool areEqual = fillFormat1.Equals(fillFormat2);

                // Karşılaştırmanın sonucunu göster
                Console.WriteLine($"FillFormat objects are equal: {areEqual}");

                // Ayrıca null ile karşılaştırmayı göster
                bool isNullEqual = fillFormat1.Equals(null);
                Console.WriteLine($"FillFormat object equals null: {isNullEqual}");

                // Çalışma kitabını kaydedin
                workbook.Save("FillEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in FillFormat Equals demonstration: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Fill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


