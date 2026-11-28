---
title: "Enum ShapeLockType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.ShapeLockType enum. Kilitlenecek özelliğin tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shapelocktype/
---
## ShapeLockType enumeration

Kilitlenecek özelliğin türünü temsil eder.

```csharp
public enum ShapeLockType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Group | `0` | Grup |
| AdjustHandles | `1` | AdjustHandles |
| Text | `2` | Metin |
| Points | `3` | Points |
| Crop | `4` | Crop |
| Selection | `5` | Selection |
| Move | `6` | Move |
| AspectRatio | `7` | AspectRatio |
| Rotation | `8` | Rotation |
| Ungroup | `9` | Ungroup |
| Resize | `10` | Resize |
| ShapeType | `11` | ShapeType |
| Arrowhead | `12` | Arrowhead |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapeLockTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir resim ekle
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[index];

            // ShapeLockType işlevselliğini gösterin
            picture.SetLockedProperty(Aspose.Cells.Drawing.ShapeLockType.AspectRatio, false);
            bool isAspectRatioLocked = picture.GetLockedProperty(Aspose.Cells.Drawing.ShapeLockType.AspectRatio);

            Console.WriteLine("Aspect Ratio locked: " + isAspectRatioLocked);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


