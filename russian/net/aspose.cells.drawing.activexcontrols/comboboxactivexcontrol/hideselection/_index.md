---
title: "ComboBoxActiveXControl.HideSelection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ComboBoxActiveXControl. Указывает, будет ли выбранный текст в элементе управления подсвечиваться, когда элемент управления не имеет фокуса"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/hideselection/
---
## ComboBoxActiveXControl.HideSelection property

Указывает, будет ли выделенный текст в элементе управления подсвечиваться, когда элемент управления не имеет фокуса.

```csharp
public bool HideSelection { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyHideSelectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить элемент управления ComboBox ActiveX со всеми необходимыми параметрами
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 
                10, 10, 150, 30, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Настройте базовые свойства
            comboBox.ListRows = 5;
            comboBox.Value = "Select an item";
            
            // Добавить образцы элементов, используя правильное имя свойства
            comboBox.ListFillRange = "A1:A3"; // Alternative way to set items
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // Продемонстрировать свойство HideSelection
            comboBox.HideSelection = true; // Text won't show selection highlight when control loses focus

            // Сохраните книгу
            workbook.Save("ComboBoxHideSelectionDemo.xlsx");
        }
    }
}
```

### См. также

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


