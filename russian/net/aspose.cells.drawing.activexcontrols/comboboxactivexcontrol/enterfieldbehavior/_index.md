---
title: "ComboBoxActiveXControl.EnterFieldBehavior"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ComboBoxActiveXControl. Указывает поведение выбора при входе в элемент управления. True указывает, что выбор остаётся неизменным с последнего раза, когда элемент управления был активен. False указывает, что весь текст в элементе управления будет выделен при входе в элемент управления."
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/enterfieldbehavior/
---
## ComboBoxActiveXControl.EnterFieldBehavior property

Указывает поведение выбора при входе в элемент управления. True указывает, что выделение остаётся неизменным с последнего раза, когда элемент управления был активен. False указывает, что весь текст в элементе управления будет выделен при входе в него.

```csharp
public bool EnterFieldBehavior { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyEnterFieldBehaviorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить первый ComboBox ActiveX Control
            Shape shape1 = worksheet.Shapes.AddActiveXControl(
                ControlType.ComboBox, 
                1, 0, 1, 0, 100, 50
            );
            ComboBoxActiveXControl combo1 = (ComboBoxActiveXControl)shape1.ActiveXControl;
            combo1.EnterFieldBehavior = false; // Default behavior (select all text on entry)
            combo1.Value = "Select Option";
            combo1.BorderStyle = ControlBorderType.Single;
            
            // Добавить второй ComboBox ActiveX Control
            Shape shape2 = worksheet.Shapes.AddActiveXControl(
                ControlType.ComboBox, 
                1, 0, 2, 0, 100, 50
            );
            ComboBoxActiveXControl combo2 = (ComboBoxActiveXControl)shape2.ActiveXControl;
            combo2.EnterFieldBehavior = true; // Preserve previous selection
            combo2.Value = "Edit Value";
            combo2.BorderStyle = ControlBorderType.Single;
            
            // Сохраните книгу
            workbook.Save("ComboBoxActiveXControlDemo.xlsm", SaveFormat.Xlsm);
            
            // Проверить настройки свойства
            Console.WriteLine("Combo1 EnterFieldBehavior: " + combo1.EnterFieldBehavior);
            Console.WriteLine("Combo2 EnterFieldBehavior: " + combo2.EnterFieldBehavior);
        }
    }
}
```

### См. также

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


