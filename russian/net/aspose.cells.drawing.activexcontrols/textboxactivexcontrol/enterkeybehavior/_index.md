---
title: "TextBoxActiveXControl.EnterKeyBehavior"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextBoxActiveXControl. Определяет поведение клавиши ENTER. True указывает, что нажатие ENTER создаст новую строку. False указывает, что нажатие ENTER переместит фокус к следующему объекту в порядке табуляции"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/enterkeybehavior/
---
## TextBoxActiveXControl.EnterKeyBehavior property

Определяет поведение клавиши ENTER. Значение True указывает, что нажатие ENTER создаст новую строку. Значение False указывает, что нажатие ENTER переместит фокус к следующему объекту в порядке табуляции.

```csharp
public bool EnterKeyBehavior { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyEnterKeyBehaviorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте элемент управления TextBox ActiveX
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 
                1, 1, 1, 1, 100, 100);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Продемонстрируйте свойство EnterKeyBehavior
            Console.WriteLine("Initial EnterKeyBehavior: " + textBox.EnterKeyBehavior);
            
            // Переключите EnterKeyBehavior
            textBox.EnterKeyBehavior = !textBox.EnterKeyBehavior;
            Console.WriteLine("Modified EnterKeyBehavior: " + textBox.EnterKeyBehavior);

            // Сохраните книгу
            workbook.Save("TextBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


