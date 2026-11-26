---
title: "Style.RotationAngle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Представляет угол поворота текста"
type: docs
url: /ru/net/aspose.cells/style/rotationangle/
---
## Style.RotationAngle property

Представляет угол поворота текста.

```csharp
public int RotationAngle { get; set; }
```

### Примечания

0: Не повернут.

255: Сверху вниз.

-90: Downward.

90: Вверх.

Вы можете установить 255 или значение в диапазоне от -90 до 90.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyRotationAngleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте стиль с разными углами поворота
            Style style1 = workbook.CreateStyle();
            style1.RotationAngle = -90;
            worksheet.Cells["B2"].PutValue("Text rotated -90°");
            worksheet.Cells["B2"].SetStyle(style1);

            Style style2 = workbook.CreateStyle();
            style2.RotationAngle = 90;
            worksheet.Cells["C3"].PutValue("Text rotated 90°");
            worksheet.Cells["C3"].SetStyle(style2);

            Style style3 = workbook.CreateStyle();
            style3.RotationAngle = 255;
            worksheet.Cells["D4"].PutValue("Text rotated 255°");
            worksheet.Cells["D4"].SetStyle(style3);

            // Сохраните книгу
            workbook.Save("output_rotation_angles.xlsx");
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


