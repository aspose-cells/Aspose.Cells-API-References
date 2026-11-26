---
title: "DataSorterKey.IconSetType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataSorterKey. Представляет тип набора значков"
type: docs
url: /ru/net/aspose.cells/datasorterkey/iconsettype/
---
## DataSorterKey.IconSetType property

Представляет тип набора значков.

```csharp
public IconSetType IconSetType { get; }
```

### Примечания

Действует только когда [`Type`](../type/) имеет значение Icon.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyIconSetTypeDemo
    {
        public static void Run()
        {
            // Создать объект рабочей книги
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте пример данных с условным форматированием набора значков
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Добавить условное форматирование набора значков
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];
            CellArea area = CellArea.CreateCellArea("A1", "A5");
            fcc.AddArea(area);
            fcc.AddCondition(FormatConditionType.IconSet);
            fcc[0].IconSet.Type = IconSetType.Arrows3;

            // Создайте сортировщик данных с типом набора значков
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Отсортировать данные
            sorter.Sort(worksheet.Cells, area);

            // Отобразите тип набора значков из ключа сортировщика
            foreach (DataSorterKey key in sorter.Keys)
            {
                Console.WriteLine($"IconSetType used for sorting: {key.IconSetType}");
            }

            // Сохраните книгу
            workbook.Save("IconSetTypeSortingDemo.xlsx");
        }
    }
}
```

### См. также

* enum [IconSetType](../../iconsettype/)
* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


