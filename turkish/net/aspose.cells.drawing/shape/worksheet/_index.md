---
title: "Shape.Worksheet"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Bu şekli içeren Worksheet nesnesini alır"
type: docs
url: /tr/net/aspose.cells.drawing/shape/worksheet/
---
## Shape.Worksheet property

Bu şekli içeren [`Worksheet`](../../../aspose.cells/worksheet/) nesnesini alır.

```csharp
public Worksheet Worksheet { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWorksheetDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            
            // Worksheet özelliğinin kullanımını gösterin
            Worksheet shapeWorksheet = shape.Worksheet;
            
            // Özelliğin çalıştığını göstermek için çalışma sayfası adını çıktıla
            Console.WriteLine("Shape belongs to worksheet: " + shapeWorksheet.Name);
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


