---
title: "ComboBoxActiveXControl.ListRows"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ComboBoxActiveXControl. Представляет максимальное количество строк для отображения в списке"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/listrows/
---
## ComboBoxActiveXControl.ListRows property

Представляет максимальное количество строк для отображения в списке.

```csharp
public int ListRows { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyListRowsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте элемент управления ComboBox ActiveX с правильными параметрами ширины/высоты
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 10, 10, 150, 30, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Добавьте образцы элементов в комбобокс, используя ListFillRange
            comboBox.ListFillRange = "A1:A7";
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");
            worksheet.Cells["A6"].PutValue("Item 6");
            worksheet.Cells["A7"].PutValue("Item 7");

            // Установите свойство ListRows, чтобы управлять видимыми элементами в раскрывающемся списке
            comboBox.ListRows = 4; // Only show 4 items at a time

            // Сохраните книгу
            workbook.Save("ComboBoxListRowsDemo.xlsx");
        }
    }
}
```

### См. также

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


