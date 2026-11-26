---
title: "Перечисление TableDataSourceType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Tables.TableDataSourceType. Представляет тип источника данных таблиц"
type: docs
url: /ru/net/aspose.cells.tables/tabledatasourcetype/
---
## TableDataSourceType enumeration

Представляет тип источника данных таблицы.

```csharp
public enum TableDataSourceType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Worksheet | `0` | Таблица листа Excel |
| SharePoint | `1` | Читаемый и записываемый связанный список SharePoint |
| XML | `2` | Таблица XML‑mapper |
| QueryTable | `3` | Таблица запросов |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableDataSourceTypeDemo
    {
        public static void TableDataSourceTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);

            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue("Charlie");

            // Добавить объект ListObject (таблицу) в лист
            int listObjectIndex = worksheet.ListObjects.Add(1, 0, 4, 1, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];

            // Установите отображаемое имя таблицы
            listObject.DisplayName = "SampleTable";

            // Установите тип источника данных таблицы
            TableDataSourceType dataSourceType = listObject.DataSourceType;

            // Выведите тип источника данных
            Console.WriteLine("Data Source Type: " + dataSourceType);

            // Сохраните книгу
            workbook.Save("TableDataSourceTypeExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


