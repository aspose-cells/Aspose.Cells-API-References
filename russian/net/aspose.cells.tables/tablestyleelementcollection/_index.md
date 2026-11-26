---
title: "Класс TableStyleElementCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Tables.TableStyleElementCollection. Представляет все элементы стиля таблицы"
type: docs
url: /ru/net/aspose.cells.tables/tablestyleelementcollection/
---
## TableStyleElementCollection class

Представляет все элементы стиля таблицы.

```csharp
public class TableStyleElementCollection : CollectionBase<TableStyleElement>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.tables/tablestyleelementcollection/item/) { get; } | Получает элемент стиля таблицы по индексу. (2 индексатора) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells.tables/tablestyleelementcollection/add/)(TableStyleElementType) | Добавляет элемент. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TableStyleElement) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TableStyleElement, IComparer&lt;TableStyleElement&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, TableStyleElement, IComparer&lt;TableStyleElement&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(TableStyleElement) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(TableStyleElement[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(TableStyleElement[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, TableStyleElement[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;TableStyleElement&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;TableStyleElement&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;TableStyleElement&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;TableStyleElement&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;TableStyleElement&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;TableStyleElement&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;TableStyleElement&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;TableStyleElement&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;TableStyleElement&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;TableStyleElement&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TableStyleElement) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TableStyleElement, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TableStyleElement, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TableStyleElement) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TableStyleElement, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TableStyleElement, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleElementCollectionDemo
    {
        public static void TableStyleElementCollectionExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Создать стили для первого и последнего столбцов
            Style firstColumnStyle = workbook.CreateStyle();
            firstColumnStyle.Pattern = BackgroundType.Solid;
            firstColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            Style lastColumnStyle = workbook.CreateStyle();
            lastColumnStyle.Font.IsBold = true;
            lastColumnStyle.Pattern = BackgroundType.Solid;
            lastColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            // Определить имя пользовательского стиля таблицы
            string tableStyleName = "Custom1";

            // Получить доступ к коллекции стилей таблицы
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

            // Добавить новый стиль таблицы в коллекцию
            int index1 = tableStyles.AddTableStyle(tableStyleName);
            TableStyle tableStyle = tableStyles[index1];

            // Получить доступ к коллекции элементов стиля таблицы
            TableStyleElementCollection elements = tableStyle.TableStyleElements;

            // Добавить и настроить элемент стиля первого столбца
            index1 = elements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement element = elements[index1];
            element.SetElementStyle(firstColumnStyle);

            // Добавить и настроить элемент стиля последнего столбца
            index1 = elements.Add(TableStyleElementType.LastColumn);
            element = elements[index1];
            element.SetElementStyle(lastColumnStyle);

            // Заполнить лист образцовыми данными
            Cells cells = workbook.Worksheets[0].Cells;
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Добавить таблицу в лист
            ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Применить пользовательский стиль таблицы к таблице.
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.TableStyleName = tableStyleName;

            // Сохраните книгу
            workbook.Save("TableStyleElementCollectionExample.xlsx");
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [TableStyleElement](../tablestyleelement/)
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


