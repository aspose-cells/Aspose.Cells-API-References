---
title: "Класс TableStyleCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Tables.TableStyleCollection. Представляет все пользовательские стили таблиц"
type: docs
url: /ru/net/aspose.cells.tables/tablestylecollection/
---
## TableStyleCollection class

Представляет все пользовательские стили таблиц.

```csharp
public class TableStyleCollection : CollectionBase<TableStyle>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [DefaultPivotStyleName](../../aspose.cells.tables/tablestylecollection/defaultpivotstylename/) { get; set; } | Получает и задает имя стиля по умолчанию сводной таблицы. |
| [DefaultTableStyleName](../../aspose.cells.tables/tablestylecollection/defaulttablestylename/) { get; set; } | Получает и задает имя стиля таблицы по умолчанию. |
| [Item](../../aspose.cells.tables/tablestylecollection/item/) { get; } | Получает стиль таблицы по индексу. (2 индексатора) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [AddPivotTableStyle](../../aspose.cells.tables/tablestylecollection/addpivottablestyle/)(string) | Добавляет пользовательский стиль сводной таблицы. |
| [AddTableStyle](../../aspose.cells.tables/tablestylecollection/addtablestyle/)(string) | Добавляет пользовательский стиль таблицы. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TableStyle) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TableStyle, IComparer&lt;TableStyle&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, TableStyle, IComparer&lt;TableStyle&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(TableStyle) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(TableStyle[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(TableStyle[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, TableStyle[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;TableStyle&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;TableStyle&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;TableStyle&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;TableStyle&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;TableStyle&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;TableStyle&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;TableStyle&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;TableStyle&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;TableStyle&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;TableStyle&gt;) |  |
| [GetBuiltinTableStyle](../../aspose.cells.tables/tablestylecollection/getbuiltintablestyle/)(TableStyleType) | Получает встроенный стиль таблицы |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TableStyle) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TableStyle, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TableStyle, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TableStyle) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TableStyle, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TableStyle, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TablesClassTableStyleCollectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к коллекции стилей таблицы
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            
            // Отобразить имена стилей по умолчанию
            Console.WriteLine("Default Table Style: " + tableStyles.DefaultTableStyleName);
            Console.WriteLine("Default Pivot Style: " + tableStyles.DefaultPivotStyleName);
            
            // Изменить стиль таблицы по умолчанию
            tableStyles.DefaultTableStyleName = "TableStyleMedium9";
            
            // Сохраните книгу
            workbook.Save("TableStylesDemo.xlsx");
            
            // Проверьте изменение, загрузив сохраненный файл
            Workbook verifyWorkbook = new Workbook("TableStylesDemo.xlsx");
            Console.WriteLine("New Default Table Style: " + 
                verifyWorkbook.Worksheets.TableStyles.DefaultTableStyleName);
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [TableStyle](../tablestyle/)
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


