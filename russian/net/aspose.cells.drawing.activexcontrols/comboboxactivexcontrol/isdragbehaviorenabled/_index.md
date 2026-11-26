---
title: "ComboBoxActiveXControl.IsDragBehaviorEnabled"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ComboBoxActiveXControl. Указывает, включено ли перетаскивание для элемента управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/isdragbehaviorenabled/
---
## ComboBoxActiveXControl.IsDragBehaviorEnabled property

Указывает, включено ли перетаскивание для элемента управления.

```csharp
public bool IsDragBehaviorEnabled { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyIsDragBehaviorEnabledDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить элемент управления ComboBox ActiveX
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 1, 0, 1, 0, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Установите некоторые базовые свойства
            comboBox.ListRows = 8;
            comboBox.ColumnCount = 1;
            comboBox.BoundColumn = 1;
            comboBox.TextColumn = -1;

            // Продемонстрировать свойство IsDragBehaviorEnabled
            Console.WriteLine("Initial IsDragBehaviorEnabled: " + comboBox.IsDragBehaviorEnabled);
            
            // Отключить перетаскивание
            comboBox.IsDragBehaviorEnabled = false;
            Console.WriteLine("After setting to false: " + comboBox.IsDragBehaviorEnabled);
            
            // Включить перетаскивание
            comboBox.IsDragBehaviorEnabled = true;
            Console.WriteLine("After setting to true: " + comboBox.IsDragBehaviorEnabled);

            // Сохраните книгу
            workbook.Save("ComboBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### См. также

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


