---
title: "AutoFilter.ShowFilterButton"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AutoFilter. Указывает, видна ли кнопка AutoFilter для этого столбца"
type: docs
url: /ru/net/aspose.cells/autofilter/showfilterbutton/
---
## AutoFilter.ShowFilterButton property

Указывает, видна ли кнопка AutoFilter для этого столбца.

```csharp
public bool ShowFilterButton { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertyShowFilterButtonDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Создать объект/таблицу списка
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];

            // Включить autofilter и показать кнопки фильтра
            table.AutoFilter.ShowFilterButton = true;

            // Сохраните книгу
            workbook.Save("output_with_filter_buttons.xlsx");

            // Скрыть кнопки фильтра
            table.AutoFilter.ShowFilterButton = false;
            workbook.Save("output_without_filter_buttons.xlsx");
        }
    }
}
```

### См. также

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


