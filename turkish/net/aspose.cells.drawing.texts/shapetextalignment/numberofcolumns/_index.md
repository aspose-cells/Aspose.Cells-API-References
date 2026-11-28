---
title: "ShapeTextAlignment.NumberOfColumns"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeTextAlignment özelliği. Sınırlayıcı dikdörtgende metnin sütun sayısını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.texts/shapetextalignment/numberofcolumns/
---
## ShapeTextAlignment.NumberOfColumns property

Sınırlayıcı dikdörtgendeki metin sütun sayısını alır ve ayarlar.

```csharp
public int NumberOfColumns { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyNumberOfColumnsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);
            
            // Şekil için metin ayarlayın
            shape.Text = "This is sample text\nin multiple columns";
            
            // Metin hizalamasına erişin ve sütun sayısını ayarlayın
            shape.TextBody.TextAlignment.NumberOfColumns = 2;
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            // Özelliği doğrula
            Console.WriteLine("Number of columns: " + 
                worksheet.Shapes[0].TextBody.TextAlignment.NumberOfColumns);
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


