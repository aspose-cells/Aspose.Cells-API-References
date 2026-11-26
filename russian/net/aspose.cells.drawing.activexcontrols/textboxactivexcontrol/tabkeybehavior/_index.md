---
title: "TextBoxActiveXControl.TabKeyBehavior"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextBoxActiveXControl. Указывает, разрешены ли символы табуляции в тексте элемента управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/tabkeybehavior/
---
## TextBoxActiveXControl.TabKeyBehavior property

Указывает, разрешены ли символы табуляции в тексте элемента управления.

```csharp
public bool TabKeyBehavior { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyTabKeyBehaviorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте TextBox ActiveX Control и получите его свойство ActiveXControl
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 100, 50);
            var textBoxControl = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Продемонстрируйте свойство TabKeyBehavior
            Console.WriteLine("Initial TabKeyBehavior: " + textBoxControl.TabKeyBehavior);
            
            // Включите TabKeyBehavior
            if (!textBoxControl.TabKeyBehavior)
            {
                textBoxControl.TabKeyBehavior = true;
                Console.WriteLine("TabKeyBehavior after setting to true: " + textBoxControl.TabKeyBehavior);
            }

            // Сохраните книгу
            workbook.Save("TextBoxActiveXControlTabKeyBehaviorDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


