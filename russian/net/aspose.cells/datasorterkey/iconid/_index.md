---
title: "DataSorterKey.IconId"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataSorterKey. Представляет идентификатор типа набора значков"
type: docs
url: /ru/net/aspose.cells/datasorterkey/iconid/
---
## DataSorterKey.IconId property

Представляет идентификатор типа набора значков.

```csharp
public int IconId { get; }
```

### Примечания

Действует только когда [`Type`](../type/) имеет значение Icon.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterKeyPropertyIconIdDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте пример данных со значениями, которые могут использовать наборы значков
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

            // Создайте сортировщик данных и добавьте ключ
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Отсортировать данные
            sorter.Sort(worksheet.Cells, area);

            try
            {
                // Отобразите свойство IconId из ключей сортировщика
                foreach (DataSorterKey key in sorter.Keys)
                {
                    Console.WriteLine($"IconId: {key.IconId}");
                    Console.WriteLine($"IconSetType: {key.IconSetType}");
                }

                // Сохраните книгу
                workbook.Save("IconIdDemo.xlsx");
                Console.WriteLine("IconId demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


