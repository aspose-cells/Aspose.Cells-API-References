---
title: "RadioButtonActiveXControl.IsWordWrapped"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RadioButtonActiveXControl. Указывает, автоматически ли содержимое элемента управления переносится в конце строки"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/iswordwrapped/
---
## RadioButtonActiveXControl.IsWordWrapped property

Указывает, будет ли содержимое контрола автоматически переноситься в конце строки.

```csharp
public bool IsWordWrapped { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class RadioButtonActiveXControlPropertyIsWordWrappedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте RadioButton ActiveX control
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton,
                1, 1, 100, 50, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl radioButton = 
                (Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl)shape.ActiveXControl;

            // Продемонстрировать свойство IsWordWrapped
            Console.WriteLine("Initial IsWordWrapped value: " + radioButton.IsWordWrapped);
            
            radioButton.IsWordWrapped = true;
            Console.WriteLine("After setting IsWordWrapped to true: " + radioButton.IsWordWrapped);
            
            radioButton.IsWordWrapped = false;
            Console.WriteLine("After setting IsWordWrapped to false: " + radioButton.IsWordWrapped);

            // Сохраните книгу
            workbook.Save("RadioButtonIsWordWrappedDemo.xlsx");
        }
    }
}
```

### См. также

* class [RadioButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


