---
title: "TextBoxActiveXControl.PasswordChar"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextBoxActiveXControl. Получает и задает символ, отображаемый вместо введённых символов"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/passwordchar/
---
## TextBoxActiveXControl.PasswordChar property

Получает и задает символ, который будет отображаться вместо введённых символов.

```csharp
public char PasswordChar { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyPasswordCharDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте TextBox ActiveX Control и получите его форму
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 0, 1, 1, 100, 50);
            
            // Получите TextBoxActiveXControl из формы
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBoxControl = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Установите свойство PasswordChar
            textBoxControl.PasswordChar = '*';

            // Установите некоторый текст, чтобы продемонстрировать маскирование пароля
            textBoxControl.Text = "password123";

            // Сохраните книгу
            workbook.Save("TextBoxActiveXControlPasswordCharDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


