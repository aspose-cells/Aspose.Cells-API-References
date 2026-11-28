---
title: "Shape.RemoveHyperlink"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape yöntemi. Şeklin hiperlinkini kaldırır"
type: docs
url: /tr/net/aspose.cells.drawing/shape/removehyperlink/
---
## Shape.RemoveHyperlink method

Şeklin hiperlinkini kaldırır.

```csharp
public void RemoveHyperlink()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodRemoveHyperlinkDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir şekil ekleyin ve hiperlinki ayarlayın
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);
            shape.AddHyperlink("https://www.aspose.com");

            // Hiperlinki kaldırın
            shape.RemoveHyperlink();

            // Hiperlinkin kaldırıldığını doğrulayın
            Console.WriteLine("Hyperlink removed: " + (shape.Hyperlink == null));

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeRemoveHyperlinkDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


