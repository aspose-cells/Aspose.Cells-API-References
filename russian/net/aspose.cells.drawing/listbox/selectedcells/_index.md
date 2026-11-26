---
title: "ListBox.SelectedCells"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListBox. Возвращает выбранные ячейки. Возвращает null, если входной диапазон не установлен или элемент не выбран"
type: docs
url: /ru/net/aspose.cells.drawing/listbox/selectedcells/
---
## ListBox.SelectedCells property

Получает выбранные ячейки. Возвращает null, если входной диапазон не установлен или элемент не выбран

```csharp
public Cell[] SelectedCells { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ListBoxPropertySelectedCellsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить примерными данными элементы ListBox
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");

            // Создать ListBox и привязать его к диапазону данных
            ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(7, 0, 100, 150, 5, 1);
            listBox.InputRange = "A1:A5";
            listBox.SelectionType = SelectionType.Multi;

            // Выбрать несколько элементов, используя индексы, начинающиеся с нуля
            listBox.SelectedItem(0, true);
            listBox.SelectedItem(2, true);

            // Получить и отобразить выбранные ячейки
            Cell[] selectedCells = listBox.SelectedCells;
            Console.WriteLine("Selected Cells Count: " + selectedCells.Length);
            
            // Изменить выбранные ячейки для демонстрации доступа
            foreach (Cell cell in selectedCells)
            {
                Console.WriteLine("Selected Cell Address: " + cell.Name);
                cell.PutValue("[SELECTED] " + cell.StringValue);
            }

            workbook.Save("ListBoxSelectedCellsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../../../aspose.cells/cell/)
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


