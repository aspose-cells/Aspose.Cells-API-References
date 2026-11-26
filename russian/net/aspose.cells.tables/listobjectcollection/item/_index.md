---
title: "ListObjectCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListObjectCollection. Получает ListObject по индексу"
type: docs
url: /ru/net/aspose.cells.tables/listobjectcollection/item/
---
## ListObjectCollection indexer (1 of 2)

Получает ListObject по индексу.

```csharp
public ListObject this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс. |

### Возвращаемое значение

Объект ListObject

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            
            // Создать объект списка
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // Доступ к объекту списка с использованием свойства Item
            ListObject firstListObject = worksheet.ListObjects[0];
            
            // Установить стиль таблицы
            firstListObject.TableStyleType = TableStyleType.TableStyleMedium2;
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [ListObject](../../listobject/)
* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## ListObjectCollection indexer (2 of 2)

Получает ListObject по указанному имени.

```csharp
public ListObject this[string tableName] { get; }
```

| Параметр | Описание |
| --- | --- |
| tableName | Имя ListObject. |

### Возвращаемое значение

Объект ListObject

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionPropertyItemDemo
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

            // Создать объект списка
            int index = worksheet.ListObjects.Add("A1", "B3", true);
            ListObject listObj = worksheet.ListObjects[index];
            listObj.DisplayName = "PersonTable";

            // Доступ к объекту списка с использованием свойства Item по имени
            ListObject retrievedListObj = worksheet.ListObjects["PersonTable"];
            
            // Продемонстрировать использование, преобразуя в диапазон
            retrievedListObj.ConvertToRange();

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [ListObject](../../listobject/)
* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


