---
title: "ComboBox.SelectedValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ComboBox. Получает выбранное значение комбобокса"
type: docs
url: /ru/net/aspose.cells.drawing/combobox/selectedvalue/
---
## ComboBox.SelectedValue property

Получает выбранное значение комбобокса.

```csharp
public string SelectedValue { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxPropertySelectedValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте ComboBox и добавьте элементы
            Aspose.Cells.Drawing.ComboBox comboBox = (Aspose.Cells.Drawing.ComboBox)worksheet.Shapes.AddComboBox(1, 0, 1, 0, 100, 50);
            comboBox.LinkedCell = "A1";
            comboBox.SetInputRange("B1:B4", false, false);
            
            // Установите значения во входном диапазоне
            worksheet.Cells["B1"].PutValue("a");
            worksheet.Cells["B2"].PutValue("b");
            worksheet.Cells["B3"].PutValue("c");
            worksheet.Cells["B4"].PutValue("d");

            // Продемонстрируйте SelectedValue (свойство только для чтения)
            Console.WriteLine("SelectedValue: " + comboBox.SelectedValue);

            // Сохраните книгу
            workbook.Save("ComboBoxDemo.xlsx");
        }
    }
}
```

### См. также

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


