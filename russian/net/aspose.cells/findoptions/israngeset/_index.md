---
title: "FindOptions.IsRangeSet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FindOptions. Указывает, установлен ли диапазон поиска"
type: docs
url: /ru/net/aspose.cells/findoptions/israngeset/
---
## FindOptions.IsRangeSet property

Указывает, установлен ли диапазон поиска.

```csharp
public bool IsRangeSet { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsPropertyIsRangeSetDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните некоторыми данными
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["B1"].PutValue("Date");
            worksheet.Cells["B2"].PutValue("Elderberry");
            worksheet.Cells["B3"].PutValue("Fig");

            // Создайте экземпляр FindOptions
            FindOptions findOptions = new FindOptions();

            // Проверьте начальное значение IsRangeSet (должно быть false)
            Console.WriteLine("Initial IsRangeSet value: " + findOptions.IsRangeSet);

            // Установите диапазон поиска
            CellArea searchRange = new CellArea();
            searchRange.StartRow = 0;
            searchRange.StartColumn = 0;
            searchRange.EndRow = 2;
            searchRange.EndColumn = 0; // Column A only
            findOptions.SetRange(searchRange);

            // Проверьте IsRangeSet после установки диапазона (должно быть true)
            Console.WriteLine("After SetRange, IsRangeSet value: " + findOptions.IsRangeSet);

            // Выполните операцию поиска в указанном диапазоне
            Cell foundCell = worksheet.Cells.Find("Banana", null, findOptions);
            Console.WriteLine("Found 'Banana' at: " + foundCell?.Name);

            // Попробуйте найти что‑то за пределами диапазона (не должно быть найдено)
            foundCell = worksheet.Cells.Find("Fig", null, findOptions);
            Console.WriteLine("Found 'Fig' at: " + foundCell?.Name); // Should be null

            // Сохраните книгу
            workbook.Save("PropertyIsRangeSetDemo.xlsx");
        }
    }
}
```

### См. также

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


