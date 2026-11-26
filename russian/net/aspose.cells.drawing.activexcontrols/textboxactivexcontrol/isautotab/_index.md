---
title: "TextBoxActiveXControl.IsAutoTab"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextBoxActiveXControl. Указывает, будет ли фокус автоматически перемещаться к следующему элементу управления, когда пользователь вводит максимальное количество символов"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isautotab/
---
## TextBoxActiveXControl.IsAutoTab property

Указывает, будет ли фокус автоматически перемещаться к следующему элементу управления, когда пользователь вводит максимальное количество символов.

```csharp
public bool IsAutoTab { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIsAutoTabDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить ActiveX‑элемент TextBox и получить его элемент управления
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 100, 30, 100, 30);
            var textBoxControl = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Продемонстрировать свойство IsAutoTab
            Console.WriteLine("Initial IsAutoTab value: " + textBoxControl.IsAutoTab);
            
            // Установить IsAutoTab в true, если он равен false
            if (!textBoxControl.IsAutoTab)
            {
                textBoxControl.IsAutoTab = true;
                Console.WriteLine("IsAutoTab set to: " + textBoxControl.IsAutoTab);
            }

            // Сохраните книгу
            workbook.Save("TextBoxActiveXControlIsAutoTabDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


