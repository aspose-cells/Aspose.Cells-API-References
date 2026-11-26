---
title: "ComboBox.SelectedIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ComboBox. Получает или задает номер индекса текущего выбранного элемента в списке или комбобоксе. Нумерация с нуля"
type: docs
url: /ru/net/aspose.cells.drawing/combobox/selectedindex/
---
## ComboBox.SelectedIndex property

Получает или задает номер индекса текущего выбранного элемента в списке или комбобоксе. Нумерация начинается с нуля.

```csharp
public int SelectedIndex { get; set; }
```

### Примечания

-1 presents no item is selected.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxPropertySelectedIndexDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для комбобокса
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");

            // Добавьте комбобокс на лист
            Shape shape = worksheet.Shapes.AddComboBox(1, 0, 1, 0, 100, 20);
            ComboBox comboBox = (ComboBox)shape;

            // Установите диапазон ввода для combo box
            comboBox.InputRange = "A1:A5";
            comboBox.DropDownLines = 5;

            // Установите и отобразите выбранный индекс
            comboBox.SelectedIndex = 2; // Selects "Item 3" (zero-based index)
            Console.WriteLine("Selected Index: " + comboBox.SelectedIndex);
            Console.WriteLine("Selected Value: " + comboBox.SelectedValue);

            // Измените выбранный индекс и отобразите снова
            comboBox.SelectedIndex = 4; // Selects "Item 5"
            Console.WriteLine("\nAfter changing selection:");
            Console.WriteLine("Selected Index: " + comboBox.SelectedIndex);
            Console.WriteLine("Selected Value: " + comboBox.SelectedValue);
        }
    }
}
```

### См. также

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


