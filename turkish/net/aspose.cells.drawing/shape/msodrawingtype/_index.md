---
title: "Shape.MsoDrawingType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Çizim tipini alır"
type: docs
url: /tr/net/aspose.cells.drawing/shape/msodrawingtype/
---
## Shape.MsoDrawingType property

Çizim tipini alır.

```csharp
public MsoDrawingType MsoDrawingType { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyMsoDrawingTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dikdörtgen şekli ekle (düzeltilmiş parametreler)
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);
            
            // Şeklin MsoDrawingType değerini al ve göster
            MsoDrawingType drawingType = rectangle.MsoDrawingType;
            Console.WriteLine("Shape MsoDrawingType: " + drawingType.ToString());

            // Çizgi şekli ekle (düzeltilmiş parametreler)
            Shape line = worksheet.Shapes.AddLine(3, 0, 3, 100, 150, 1);
            
            // Çizginin MsoDrawingType değerini al ve göster
            drawingType = line.MsoDrawingType;
            Console.WriteLine("Line MsoDrawingType: " + drawingType.ToString());
        }
    }
}
```

### Ayrıca Bakınız

* enum [MsoDrawingType](../../msodrawingtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


