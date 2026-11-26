---
title: "Класс ColumnCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.ColumnCollection class. Коллекция объектов Column, представляющих отдельные настройки столбцов в листе. Объект Column представляет только такие настройки, как ширина столбца, стили и т.д., и не имеет отношения к тому, есть ли в соответствующем столбце непустые данные ячеек или нет. Свойство Count этой коллекции представляет только количество объектов Column, созданных в этой коллекции, и также не связано с тем, есть ли в листе непустые данные ячеек."
type: docs
url: /ru/net/aspose.cells/columncollection/
---
## ColumnCollection class

Коллекция объектов [`Column`](../column/) , представляющих отдельные column(setting)s в листе. Объект Column только представляет такие настройки, как ширина столбца, стили и т.д., и не имеет отношения к тому, есть ли в соответствующем столбце непустые данные ячеек или нет. А \"Count\" этой коллекции только представляет количество объектов Column, созданных в этой коллекции, и также не связано с тем, есть ли в листе непустые данные ячеек.

```csharp
public class ColumnCollection : CollectionBase<Column>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/columncollection/item/) { get; } | Получает объект [`Column`](../column/) по индексу столбца. Объект Column указанного индекса будет создан, если он ранее не существовал. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Column) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Column, IComparer&lt;Column&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Column, IComparer&lt;Column&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Column) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Column[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Column[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Column[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Column&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Column&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Column&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Column&gt;) |  |
| [GetByIndex](../../aspose.cells/columncollection/getbyindex/)(int) | (**Obsolete.**) Получает объект столбца по индексу. |
| [GetColumnByIndex](../../aspose.cells/columncollection/getcolumnbyindex/)(int) | Получает объект [`Column`](../column/) по позиции в списке. |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Column) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Column, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Column, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Column) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Column, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Column, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnCollectionDemo
    {
        public static void ColumnCollectionExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();

            // Получение ссылки на первый лист
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить новый Style в Workbook
            Style style = workbook.CreateStyle();

            // Установка фонового цвета в синий
            style.ForegroundColor = Color.Blue;

            // Установка фонового узора
            style.Pattern = BackgroundType.Solid;

            // Новый флаг стиля
            StyleFlag styleFlag = new StyleFlag();

            // Установить все стили
            styleFlag.All = true;

            // Изменить ширину по умолчанию первых десяти столбцов
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells.Columns[i].Width = 20;
            }

            // Получить Column с нестандартным форматированием
            ColumnCollection columns = worksheet.Cells.Columns;

            foreach (Column column in columns)
            {
                // Применить Style к первым десяти Columns
                column.ApplyStyle(style, styleFlag);
            }

            // Сохранение файла Excel
            workbook.Save("ColumnCollectionExample.xlsx");
            workbook.Save("ColumnCollectionExample.pdf");
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Column](../column/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


