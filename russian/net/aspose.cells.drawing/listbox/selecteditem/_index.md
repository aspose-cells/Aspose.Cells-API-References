---
title: "ListBox.SelectedItem"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ListBox. Устанавливает, выбран ли элемент"
type: docs
url: /ru/net/aspose.cells.drawing/listbox/selecteditem/
---
## ListBox.SelectedItem method

Устанавливает, выбран ли элемент

```csharp
public void SelectedItem(int itemIndex, bool isSelected)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| itemIndex | Int32 | Индекс элемента |
| isSelected | Boolean | Указывает, выбран ли элемент. True означает, что элемент должен быть выбран. False означает, что элемент должен быть снят с выбора. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ListBoxMethodSelectedItemWithInt32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить элементы списка
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[i, 0].Value = $"Item {i + 1}";
            }

            // Создать list box
            ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 1, 1, 150, 100) as ListBox;
            listBox.InputRange = "A1:A5";
            listBox.SelectionType = SelectionType.Multi;

            try
            {
                // Выбрать и снять выбор с элементов
                listBox.SelectedItem(2, true);  // Select third item (index 2)
                listBox.SelectedItem(0, true);   // Select first item (index 0)
                listBox.SelectedItem(2, false); // Deselect third item

                // Проверить выбранные элементы
                Console.WriteLine($"Item 0 selected: {listBox.IsSelected(0)}");
                Console.WriteLine($"Item 2 selected: {listBox.IsSelected(2)}");

                // Отобразить выбранные ячейки
                Console.WriteLine("\nSelected Items:");
                foreach (Cell cell in listBox.SelectedCells)
                {
                    Console.WriteLine(cell.Value);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("ListBoxMethodSelectedItemWithInt32BooleanDemo.xlsx");
        }
    }
}
```

### См. также

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


