---
title: "Enum LightRigDirectionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.LightRigDirectionType enum. Işık çerçevesi yön tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/lightrigdirectiontype/
---
## LightRigDirectionType enumeration

Işık çerçevesi yön tipini temsil eder.

```csharp
public enum LightRigDirectionType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Bottom | `0` | Alt |
| BottomLeft | `1` | Sol alt. |
| BottomRight | `2` | Alt Sağ. |
| Left | `3` | Sol. |
| Right | `4` | Sağ. |
| Top | `5` | Üst. |
| TopLeft | `6` | Sol üst. |
| TopRight | `7` | Üst Sağ. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassLightRigDirectionTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Işık çerçevesi yönünü göstermek için bir şekil ekleyin
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 200, 0, 0);

            // Şeklin 3B formatı için ışık çerçevesi yönünü ayarlayın
            shape.ThreeDFormat.LightingDirection = LightRigDirectionType.TopRight;

            // Farklı ışık çerçevesi yönlerini gösterin
            Console.WriteLine("Current Light Rig Direction: " + shape.ThreeDFormat.LightingDirection);

            // Işık çerçevesi yönünü değiştirin
            shape.ThreeDFormat.LightingDirection = LightRigDirectionType.BottomLeft;
            Console.WriteLine("Changed Light Rig Direction: " + shape.ThreeDFormat.LightingDirection);

            // Tüm olası ışık çerçevesi yönleri arasında yineleyin
            Console.WriteLine("\nAll Light Rig Direction Types:");
            foreach (LightRigDirectionType direction in Enum.GetValues(typeof(LightRigDirectionType)))
            {
                Console.WriteLine(direction.ToString());
            }

            // Çalışma kitabını kaydedin
            workbook.Save("LightRigDirectionTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


