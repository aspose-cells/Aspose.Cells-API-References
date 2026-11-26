---
title: "TextBoxActiveXControl.HideSelection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextBoxActiveXControl. Указывает, отображается ли выделенный текст в элементе управления подсвеченным, когда элемент управления не имеет фокуса"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/hideselection/
---
## TextBoxActiveXControl.HideSelection property

Указывает, будет ли выделенный текст в элементе управления подсвечиваться, когда элемент управления не имеет фокуса.

```csharp
public bool HideSelection { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyHideSelectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте элемент управления ActiveX TextBox на лист
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 100, 50);
            var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Продемонстрировать свойство HideSelection
            Console.WriteLine("Initial HideSelection value: " + textBox.HideSelection);
            
            // Установите HideSelection в true, если оно равно false
            if (!textBox.HideSelection)
            {
                textBox.HideSelection = true;
                Console.WriteLine("HideSelection set to: " + textBox.HideSelection);
            }

            // Сохраните книгу
            workbook.Save("TextBoxActiveXControlHideSelectionDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


