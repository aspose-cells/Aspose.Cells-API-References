---
title: "TextBoxActiveXControl.DropButtonStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextBoxActiveXControl. Указывает символ, отображаемый на кнопке раскрытия"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/dropbuttonstyle/
---
## TextBoxActiveXControl.DropButtonStyle property

Указывает символ, отображаемый на кнопке раскрытия

```csharp
public DropButtonStyle DropButtonStyle { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyDropButtonStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте элемент управления TextBox ActiveX
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.TextBox, 1, 1, 100, 50, 100, 50);
            ActiveXControl control = shape.ActiveXControl;
            
            // Преобразуйте к TextBoxActiveXControl, чтобы получить доступ к специфическим свойствам TextBox
            TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)control;
            
            // Задайте свойство DropButtonStyle
            textBoxControl.DropButtonStyle = DropButtonStyle.Arrow;
            
            // Сохраните книгу
            workbook.Save("TextBoxActiveXControlDropButtonStyleDemo.xlsx");
        }
    }
}
```

### См. также

* enum [DropButtonStyle](../../dropbuttonstyle/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


