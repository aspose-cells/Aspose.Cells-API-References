---
title: "ComboBoxActiveXControl.IsEditable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ComboBoxActiveXControl. Указывает, может ли пользователь вводить текст в элемент управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/iseditable/
---
## ComboBoxActiveXControl.IsEditable property

Указывает, может ли пользователь вводить текст в элемент управления.

```csharp
public bool IsEditable { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyIsEditableDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить элемент управления ComboBox ActiveX с использованием коллекции Shapes
            Shape shape = sheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 5, 0, 100, 30);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Установите свойства для ComboBox
            comboBox.IsEditable = true;
            comboBox.Value = "Editable ComboBox";
            comboBox.ColumnCount = 2;
            comboBox.ListRows = 6;
            comboBox.TextColumn = 1;

            // Добавить элементы в ComboBox (используя свойство ListFillRange)
            sheet.Cells["A10"].PutValue("Item 1");
            sheet.Cells["B10"].PutValue("Description 1");
            sheet.Cells["A11"].PutValue("Item 2");
            sheet.Cells["B11"].PutValue("Description 2");
            comboBox.ListFillRange = "A10:B11";

            // Сохраните книгу
            workbook.Save("ComboBoxActiveXControl_IsEditableDemo.xlsx");

            // Проверить свойство после сохранения
            Console.WriteLine("IsEditable property value: " + comboBox.IsEditable);
        }
    }
}
```

### См. также

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


