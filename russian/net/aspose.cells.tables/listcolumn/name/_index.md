---
title: "ListColumn.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListColumn. Получает и задает имя столбца"
type: docs
url: /ru/net/aspose.cells.tables/listcolumn/name/
---
## ListColumn.Name property

Получает и задает имя столбца.

```csharp
public string Name { get; set; }
```

### Примечания

Если задается имя столбца, соответствующее значение ячейки также будет изменено.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать примерные данные
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Value");
            
            // Создать объект таблицы/списка
            int index = worksheet.ListObjects.Add(0, 0, 2, 2, true);
            Aspose.Cells.Tables.ListObject listObject = worksheet.ListObjects[index];

            // Получить доступ и изменить свойство Name первого столбца списка
            listObject.ListColumns[0].Name = "NewID";
            
            // Проверьте, что имя было установлено
            Console.WriteLine("First column name: " + listObject.ListColumns[0].Name);
            
            // Сохраните книгу
            workbook.Save("ListColumnPropertyNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


