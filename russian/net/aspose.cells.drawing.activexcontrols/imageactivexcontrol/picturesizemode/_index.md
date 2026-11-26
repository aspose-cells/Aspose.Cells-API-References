---
title: "ImageActiveXControl.PictureSizeMode"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageActiveXControl. Получает и задает способ отображения изображения"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/picturesizemode/
---
## ImageActiveXControl.PictureSizeMode property

Получает и задает способ отображения изображения.

```csharp
public ControlPictureSizeMode PictureSizeMode { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyPictureSizeModeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте элемент управления Image ActiveX на лист
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 1, 200, 200, 0, 0);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // Установите PictureSizeMode и другие свойства
            imageControl.PictureSizeMode = ControlPictureSizeMode.Stretch;
            
            // Загрузите образец изображения (замените на свой путь к изображению)
            string imagePath = "sample.jpg";
            if (File.Exists(imagePath))
            {
                byte[] imageData = File.ReadAllBytes(imagePath);
                imageControl.Picture = imageData;
            }

            // Сохраните книгу
            workbook.Save("ImageActiveXControlDemo.xlsx");

            // Выведите значение PictureSizeMode
            Console.WriteLine($"PictureSizeMode: {imageControl.PictureSizeMode}");
        }
    }
}
```

### См. также

* enum [ControlPictureSizeMode](../../controlpicturesizemode/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


