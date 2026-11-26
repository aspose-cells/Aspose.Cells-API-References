---
title: "DataSorter.SortLeftToRight"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataSorter. True означает, что ориентация сортировки слева направо. False означает, что ориентация сортировки сверху вниз. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/datasorter/sortlefttoright/
---
## DataSorter.SortLeftToRight property

True означает, что ориентация сортировки слева направо. False означает, что ориентация сортировки сверху вниз. Значение по умолчанию — false.

```csharp
public bool SortLeftToRight { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertySortLeftToRightDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Пример данных (столбцы будут рассматриваться как строки, когда SortLeftToRight=true)
            worksheet.Cells["A1"].PutValue(3);
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B1"].PutValue("C");
            worksheet.Cells["B2"].PutValue("A");
            worksheet.Cells["B3"].PutValue("B");

            // Создайте сортировщик данных и установите сортировку слева направо
            DataSorter sorter = workbook.DataSorter;
            sorter.SortLeftToRight = true;

            // Установите ключ сортировки (индекс столбца становится индексом строки при сортировке слева направо)
            sorter.Key1 = 0; // Sort by first "row" (originally column A)

            // Определите область сортировки (строки становятся столбцами при сортировке слева направо)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 2;
            area.StartColumn = 0;
            area.EndColumn = 1;

            // Выполните сортировку
            sorter.Sort(worksheet.Cells, area);

            // Сохранить результат
            workbook.Save("SortedLeftToRight.xlsx");
        }
    }
}
```

### См. также

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


