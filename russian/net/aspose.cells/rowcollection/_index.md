---
title: "Класс RowCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.RowCollection. Содержит объекты Row, представляющие отдельные строки в листе"
type: docs
url: /ru/net/aspose.cells/rowcollection/
---
## RowCollection class

Собирает объекты [`Row`](../row/), представляющие отдельные строки в листе.

```csharp
public class RowCollection : IEnumerable
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.cells/rowcollection/count/) { get; } | Возвращает количество строк в этой коллекции. |
| [Item](../../aspose.cells/rowcollection/item/) { get; } | Получает объект [`Row`](../row/) по заданному индексу строки. Объект Row с указанным индексом будет создан, если он ранее не существовал. |

## Методы

| Имя | Описание |
| --- | --- |
| [Clear](../../aspose.cells/rowcollection/clear/)() | Очистить все строки и ячейки. |
| [GetEnumerator](../../aspose.cells/rowcollection/getenumerator/#getenumerator)() | Возвращает перечислитель, который перебирает строки в этой коллекции |
| [GetEnumerator](../../aspose.cells/rowcollection/getenumerator/#getenumerator_1)(bool, bool) | Возвращает перечислитель, который перебирает строки в этой коллекции |
| [GetRowByIndex](../../aspose.cells/rowcollection/getrowbyindex/)(int) | Получает объект строки по позиции в списке. |
| [RemoveAt](../../aspose.cells/rowcollection/removeat/)(int) | Удаляет элемент строки по указанному индексу (позиции) в этой коллекции. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RowCollectionDemo
    {
        public static void RowCollectionExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();

            // Получение ссылки на первый лист
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");
            worksheet.Cells["A3"].PutValue("Aspose.Cells");
            // Получить коллекцию Rows
            RowCollection rows = worksheet.Cells.Rows;

            // Получить количество строк в коллекции
            int rowCount = rows.Count;
            Console.WriteLine("Number of rows: " + rowCount);

            // Получить первую строку
            Row firstRow = rows[0];
            Console.WriteLine("First row index: " + firstRow.Index);

            // Перебрать строки с помощью GetEnumerator
            IEnumerator enumerator = rows.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Row row = (Row)enumerator.Current;
                Console.WriteLine("Row index: " + row.Index + ", Height: " + row.Height);
            }

            // Получить строку по индексу
            Row specificRow = rows.GetRowByIndex(1);
            Console.WriteLine("Specific row index: " + specificRow.Index);

            // Очистить все строки и ячейки
            rows.Clear();
            Console.WriteLine("Rows cleared.");

            // Сохраните книгу
            workbook.Save("RowCollectionExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


