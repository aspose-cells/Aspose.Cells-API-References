---
title: "ShapeCollection.UpdateSelectedValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Обновляет выбранное значение значением связанной ячейки или диапазона формы"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/updateselectedvalue/
---
## ShapeCollection.UpdateSelectedValue method

Обновить выбранное значение значением связанной ячейки или диапазона фигуры.

```csharp
public void UpdateSelectedValue()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodUpdateSelectedValueDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте форму (выпадающий список) на лист
            Aspose.Cells.Drawing.ListBox listBox = (Aspose.Cells.Drawing.ListBox)worksheet.Shapes.AddListBox(0, 0, 100, 100, 3, 20);
            
            // Установите элементы списка и выбранное значение
            listBox.SetInputRange("A1:A3", false, false);
            listBox.SelectedIndex = 1;
            
            // Обновите выбранное значение в форме
            worksheet.Shapes.UpdateSelectedValue();
            
            // Сохраните книгу
            workbook.Save("ShapeCollectionUpdateSelectedValueDemo.xlsx");
        }
    }
}
```

### См. также

* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


