---
title: "Перечисление ControlPictureAlignmentType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.ActiveXControls.ControlPictureAlignmentType. Представляет выравнивание изображения внутри формы или изображения"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/controlpicturealignmenttype/
---
## ControlPictureAlignmentType enumeration

Представляет выравнивание изображения внутри Form или Image.

```csharp
public enum ControlPictureAlignmentType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| TopLeft | `0` | Верхний левый угол. |
| TopRight | `1` | Верхний правый угол. |
| Center | `2` | Центр. |
| BottomLeft | `3` | Нижний левый угол. |
| BottomRight | `4` | Нижний правый угол. |

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlsClassControlPictureAlignmentTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте ImageActiveXControl со всеми необходимыми параметрами
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.Image, 
                10,  // left
                10,  // top
                200, // width
                200, // height
                0,   // imageWidth
                0    // imageHeight
            );
            Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl = 
                (Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;

            // Установите свойства изображения
            imageControl.Picture = File.ReadAllBytes("sample.png");
            imageControl.PictureAlignment = Aspose.Cells.Drawing.ActiveXControls.ControlPictureAlignmentType.Center;
            imageControl.PictureSizeMode = Aspose.Cells.Drawing.ActiveXControls.ControlPictureSizeMode.Stretch;

            // Сохраните книгу
            workbook.Save("ImageControlDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


