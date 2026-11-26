---
title: "TextBoxActiveXControl.EnterFieldBehavior"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextBoxActiveXControl. Определяет поведение выделения при входе в элемент управления. True указывает, что выделение остаётся неизменным с последнего раза, когда элемент был активен. False указывает, что весь текст в элементе будет выделен при входе в элемент управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/enterfieldbehavior/
---
## TextBoxActiveXControl.EnterFieldBehavior property

Указывает поведение выбора при входе в элемент управления. True указывает, что выделение остаётся неизменным с последнего раза, когда элемент управления был активен. False указывает, что весь текст в элементе управления будет выделен при входе в него.

```csharp
public bool EnterFieldBehavior { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyEnterFieldBehaviorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте элемент управления TextBox ActiveX с правильными параметрами
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 
                1, 1, 1, 1, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Продемонстрируйте свойство EnterFieldBehavior
            Console.WriteLine("Initial EnterFieldBehavior: " + textBox.EnterFieldBehavior);
            
            // Переключите свойство EnterFieldBehavior
            textBox.EnterFieldBehavior = !textBox.EnterFieldBehavior;
            Console.WriteLine("Toggled EnterFieldBehavior: " + textBox.EnterFieldBehavior);

            // Явно задайте EnterFieldBehavior значение true
            textBox.EnterFieldBehavior = true;
            Console.WriteLine("Final EnterFieldBehavior: " + textBox.EnterFieldBehavior);
        }
    }
}
```

### См. также

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


