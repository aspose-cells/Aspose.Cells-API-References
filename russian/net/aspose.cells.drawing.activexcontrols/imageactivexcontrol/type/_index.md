---
title: "ImageActiveXControl.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageActiveXControl. Получает тип элемента управления ActiveX"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/type/
---
## ImageActiveXControl.Type property

Получает тип ActiveX‑элемента управления.

```csharp
public override ControlType Type { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте элемент управления Image ActiveX
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 1, 1, 1, 200, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;
            
            // Продемонстрировать использование свойства Type
            Console.WriteLine("Control Type: " + imageControl.Type);
            
            // Установите некоторые свойства
            imageControl.IsAutoSize = false;
            imageControl.BorderStyle = ControlBorderType.Single;
            imageControl.PictureSizeMode = ControlPictureSizeMode.Clip;
            
            // Сохраните книгу
            workbook.Save("ImageActiveXControlDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ControlType](../../controltype/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


