---
title: "Shape.ControlData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Kontrolün verilerini alır"
type: docs
url: /tr/net/aspose.cells.drawing/shape/controldata/
---
## Shape.ControlData property

Denetimin verisini alır.

```csharp
public byte[] ControlData { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyControlDataDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğru parametrelerle bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            
            // ControlData'ya eriş (yalnızca okuma özelliği)
            byte[] controlData = shape.ControlData;

            // ControlData'yı kontrol et
            if (controlData != null)
            {
                Console.WriteLine("ControlData exists with length: " + controlData.Length);
            }
            else
            {
                Console.WriteLine("No data.");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


