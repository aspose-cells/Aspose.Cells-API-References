---
title: "ImageActiveXControl.IsTiled"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageActiveXControl. Указывает, будет ли изображение заполнять фон плиткой"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/istiled/
---
## ImageActiveXControl.IsTiled property

Указывает, будет ли изображение замощено по фону.

```csharp
public bool IsTiled { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyIsTiledDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте элемент управления Image ActiveX на лист
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 5, 0, 1, 1, 100, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // Установите свойство IsTiled и другие свойства
            imageControl.IsTiled = true;
            imageControl.PictureSizeMode = ControlPictureSizeMode.Stretch;

            // Загрузите изображение из файла (замените на свой путь к изображению)
            byte[] imageData = File.ReadAllBytes("demo.jpg");
            imageControl.Picture = imageData;

            // Сохраните книгу
            workbook.Save("ImageActiveXControlIsTiledDemo.xlsx");

            Console.WriteLine($"IsTiled property set to: {imageControl.IsTiled}");
        }
    }
}
```

### См. также

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


