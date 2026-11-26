---
title: "ImageActiveXControl.SpecialEffect"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageActiveXControl. Получает и задает специальный эффект элемента управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/specialeffect/
---
## ImageActiveXControl.SpecialEffect property

Получает и задает специальный эффект элемента управления.

```csharp
public ControlSpecialEffectType SpecialEffect { get; set; }
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
    public class ImageActiveXControlPropertySpecialEffectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 5, 0, 1, 1, 100, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // Продемонстрировать свойство SpecialEffect
            imageControl.SpecialEffect = ControlSpecialEffectType.Raised;
            
            // Установите другие необходимые свойства
            imageControl.BorderStyle = ControlBorderType.Single;
            byte[] imageData = File.ReadAllBytes("demo.jpg");
            imageControl.Picture = imageData;

            workbook.Save("ImageActiveXControlSpecialEffectDemo.xlsx");
            
            Console.WriteLine($"SpecialEffect set to: {imageControl.SpecialEffect}");
        }
    }
}
```

### См. также

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


