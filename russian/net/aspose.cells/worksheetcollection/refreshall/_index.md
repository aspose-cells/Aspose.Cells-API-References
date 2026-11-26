---
title: "WorksheetCollection.RefreshAll"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WorksheetCollection. Обновить все сводные таблицы и диаграммы с источником сводных данных"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/refreshall/
---
## WorksheetCollection.RefreshAll method

Обновить все сводные таблицы и диаграммы с источником сводных данных.

```csharp
[Obsolete("Use Workbook.RefreshAll() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void RefreshAll()
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод Workbook.RefreshAll(). Этот метод будет удалён через 12 месяцев, начиная с апреля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRefreshAllDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные и формулы
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["B3"].PutValue(1.8);
            
            // Добавить формулы, которые будут обновлены
            worksheet.Cells["C1"].PutValue("Total");
            worksheet.Cells["C2"].PutValue("=SUM(B2:B3)");
            
            // Изменить некоторые значения
            worksheet.Cells["B2"].PutValue(3.0);
            worksheet.Cells["B3"].PutValue(2.0);
            
            // Обновить все формулы во всех листах
            workbook.Worksheets.RefreshAll();
            
            // Вывести обновлённый итог
            Console.WriteLine("Refreshed total: " + worksheet.Cells["C2"].StringValue);
        }
    }
}
```

### См. также

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


