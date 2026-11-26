---
title: "ComboBoxActiveXControl.Value"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ComboBoxActiveXControl. Получает и задает значение элемента управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/value/
---
## ComboBoxActiveXControl.Value property

Получает и задает значение элемента управления.

```csharp
public string Value { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте элемент управления ComboBox ActiveX на лист
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 1, 1, 0, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Установите свойства для ComboBox
            comboBox.Value = "Initial Value";
            comboBox.ListFillRange = "A1:A3";
            
            // Добавьте некоторые образцы данных в диапазон списка
            worksheet.Cells["A1"].PutValue("Option 1");
            worksheet.Cells["A2"].PutValue("Option 2");
            worksheet.Cells["A3"].PutValue("Option 3");

            // Обновите выбранное значение из связанной ячейки
            worksheet.Cells["B1"].PutValue("Option 2");
            worksheet.Shapes.UpdateSelectedValue();

            // Продемонстрировать получение свойства Value
            Console.WriteLine("ComboBox Value: " + comboBox.Value);

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


