---
title: "ImageActiveXControl.IsAutoSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageActiveXControl. Указывает, будет ли элемент управления автоматически изменять размер для отображения всего содержимого"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/isautosize/
---
## ImageActiveXControl.IsAutoSize property

Указывает, будет ли элемент управления автоматически изменять размер для отображения всего содержимого.

```csharp
public override bool IsAutoSize { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyIsAutoSizeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить ImageActiveXControl на лист
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.Image, 
                5,  // left
                5,  // top
                100, // width
                100, // height
                0,   // imageWidth (0 for default)
                0    // imageHeight (0 for default)
            );
            Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl = 
                (Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;

            // Установите данные изображения (убедитесь, что файл изображения существует)
            imageControl.Picture = File.ReadAllBytes("ControlPictureSizeMode.png");

            // Продемонстрировать свойство IsAutoSize
            imageControl.IsAutoSize = true; // Control will automatically resize to fit the image
            imageControl.PictureSizeMode = Aspose.Cells.Drawing.ActiveXControls.ControlPictureSizeMode.Zoom;

            // Сохраните книгу
            workbook.Save("ImageActiveXControlIsAutoSizeDemo.xlsx");
        }
    }
}
```

### См. также

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


