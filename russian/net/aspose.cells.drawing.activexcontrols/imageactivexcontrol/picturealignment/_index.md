---
title: "ImageActiveXControl.PictureAlignment"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageActiveXControl. Получает и задает выравнивание изображения внутри формы или изображения"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/picturealignment/
---
## ImageActiveXControl.PictureAlignment property

Получает и задает выравнивание изображения внутри формы или картинки.

```csharp
public ControlPictureAlignmentType PictureAlignment { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyPictureAlignmentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.Image, 5, 0, 1, 1, 100, 100);
            Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl = (Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;

            // Установите свойство PictureAlignment
            imageControl.PictureAlignment = Aspose.Cells.Drawing.ActiveXControls.ControlPictureAlignmentType.Center;

            // Загрузите образец изображения (замените на фактический путь к изображению)
            string imagePath = "sample.jpg";
            if (File.Exists(imagePath))
            {
                byte[] imageData = File.ReadAllBytes(imagePath);
                imageControl.Picture = imageData;
            }

            workbook.Save("ImageActiveXControlDemo.xlsx");

            Console.WriteLine($"PictureAlignment: {imageControl.PictureAlignment}");
        }
    }
}
```

### См. также

* enum [ControlPictureAlignmentType](../../controlpicturealignmenttype/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


