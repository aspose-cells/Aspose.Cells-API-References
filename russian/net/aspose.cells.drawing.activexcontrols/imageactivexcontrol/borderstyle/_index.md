---
title: "ImageActiveXControl.BorderStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageActiveXControl. Получает и задает тип границы, используемой элементом управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/borderstyle/
---
## ImageActiveXControl.BorderStyle property

Получает и задает тип границы, используемой элементом управления.

```csharp
public ControlBorderType BorderStyle { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyBorderStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.Image, 
                5, 5, 100, 100, 200, 200);
            Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl = 
                (Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;

            // Установите стиль границы и продемонстрируйте его использование
            imageControl.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.Single;
            imageControl.BorderOleColor = 0x000000; // Black border

            // Установите образец изображения (убедитесь, что этот файл существует в каталоге выполнения)
            if (File.Exists("sample.png"))
            {
                imageControl.Picture = File.ReadAllBytes("sample.png");
            }

            workbook.Save("ImageActiveXControlBorderStyleDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ControlBorderType](../../controlbordertype/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


