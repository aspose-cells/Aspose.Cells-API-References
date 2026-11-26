---
title: "LabelActiveXControl.Picture"
second_title: "Справочник API Aspose.Cells для .NET"
description: "LabelActiveXControl property. Получает и задает данные изображения"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/picture/
---
## LabelActiveXControl.Picture property

Получает и задает данные изображения.

```csharp
public byte[] Picture { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.IO;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertyPictureDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте Label ActiveX control
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 1, 1, 1, 1, 100, 50);
            LabelActiveXControl labelControl = (LabelActiveXControl)shape.ActiveXControl;

            // Установите базовые свойства
            labelControl.Caption = "Sample Label";
            labelControl.PicturePosition = ControlPicturePositionType.LeftTop;

            // Загрузить изображение для свойства Picture
            string imagePath = "sample.jpg"; // Replace with actual image path
            if (File.Exists(imagePath))
            {
                labelControl.Picture = File.ReadAllBytes(imagePath);
                Console.WriteLine("Picture set successfully");
            }
            else
            {
                Console.WriteLine("Image file not found, using null picture");
                labelControl.Picture = null;
            }

            // Сохраните книгу
            workbook.Save("LabelActiveXControlDemo.xlsx");
        }
    }
}
```

### См. также

* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


