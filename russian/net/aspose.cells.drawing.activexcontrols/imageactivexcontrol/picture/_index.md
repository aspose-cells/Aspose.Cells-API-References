---
title: "ImageActiveXControl.Picture"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageActiveXControl. Получает и задает данные изображения"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/picture/
---
## ImageActiveXControl.Picture property

Получает и задает данные изображения.

```csharp
public byte[] Picture { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyPictureDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте Image ActiveX control
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 1, 100, 100, 100, 100);
            ImageActiveXControl imgControl = (ImageActiveXControl)shape.ActiveXControl;

            // Установить свойства
            imgControl.PictureSizeMode = ControlPictureSizeMode.Stretch;
            imgControl.PictureAlignment = ControlPictureAlignmentType.TopLeft;
            imgControl.IsTiled = false;

            // Установите свойство Picture (используя массив байтов образца изображения)
            byte[] imageData = new byte[] { 0x00, 0x01, 0x02 }; // Sample image data
            imgControl.Picture = imageData;

            // Проверьте, что свойство Picture было установлено
            Console.WriteLine("Picture data length: " + imgControl.Picture.Length);

            // Сохраните книгу
            workbook.Save("ImageActiveXControlDemo.xlsx");
        }
    }
}
```

### См. также

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


