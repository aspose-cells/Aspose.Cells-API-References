---
title: "ListColumnCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListColumnCollection. Получает ListColumn по индексу"
type: docs
url: /ru/net/aspose.cells.tables/listcolumncollection/item/
---
## ListColumnCollection indexer (1 of 2)

Получает ListColumn по индексу.

```csharp
public ListColumn this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс. |

### Возвращаемое значение

объект ListColumn.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("T1");
            worksheet.Cells["B1"].PutValue("T2");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(2);

            // Создать объект списка
            int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
            ListObject listObj = worksheet.ListObjects[index];
            
            // Доступ к колонкам списка с помощью свойства Item
            ListColumn firstColumn = listObj.ListColumns[0];
            Console.WriteLine("First column name: " + firstColumn.Name);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [ListColumn](../../listcolumn/)
* class [ListColumnCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## ListColumnCollection indexer (2 of 2)

Получает ListColumn по имени.

```csharp
public ListColumn this[string name] { get; }
```

| Параметр | Описание |
| --- | --- |
| name | Имя ListColumn |

### Возвращаемое значение

Объект ListColumn.

### См. также

* class [ListColumn](../../listcolumn/)
* class [ListColumnCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


