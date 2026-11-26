---
title: "RadioButtonActiveXControl.Alignment"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RadioButtonActiveXControl. Получает и задает положение подписи относительно элемента управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/alignment/
---
## RadioButtonActiveXControl.Alignment property

Получает и задает положение подписи относительно контрола.

```csharp
public ControlCaptionAlignmentType Alignment { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class RadioButtonActiveXControlPropertyAlignmentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать новую коллекцию фигур и добавить ActiveX‑контрол
            ShapeCollection shapes = worksheet.Shapes;
            Shape shape = shapes.AddActiveXControl(ControlType.RadioButton, 1, 1, 100, 30, 0, 0);
            RadioButtonActiveXControl radioButton = (RadioButtonActiveXControl)shape.ActiveXControl;
            
            // Установить свойство Alignment
            radioButton.Alignment = ControlCaptionAlignmentType.Left;
            
            // Сохраните книгу
            workbook.Save("RadioButtonAlignmentDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ControlCaptionAlignmentType](../../controlcaptionalignmenttype/)
* class [RadioButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


