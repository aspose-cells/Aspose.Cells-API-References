---
title: "CheckBoxCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CheckBoxCollection. Возвращает элемент CheckBox по указанному индексу"
type: docs
url: /ru/net/aspose.cells.drawing/checkboxcollection/item/
---
## CheckBoxCollection indexer

Получает элемент [`CheckBox`](../../checkbox/) по указанному индексу.

```csharp
public CheckBox this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс элемента, начиная с нуля. |

### Возвращаемое значение

Элемент по указанному индексу.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить флажок на лист
            int index = worksheet.CheckBoxes.Add(10, 10, 100, 20);
            
            // Доступ к checkbox через свойство Item (индексатор)
            Aspose.Cells.Drawing.CheckBox checkBox = worksheet.CheckBoxes[index];
            checkBox.Text = "Sample CheckBox";
            checkBox.Name = "CheckBox1";
            
            // Доступ к checkbox через индекс (свойство Item)
            Aspose.Cells.Drawing.CheckBox checkBoxByName = worksheet.CheckBoxes[0];
            
            // Выведите свойства checkbox
            Console.WriteLine("CheckBox Name: " + checkBoxByName.Name);
            Console.WriteLine("CheckBox Text: " + checkBoxByName.Text);
            
            // Сохраните книгу
            workbook.Save("CheckBoxExample.xlsx");
        }
    }
}
```

### См. также

* class [CheckBox](../../checkbox/)
* class [CheckBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


