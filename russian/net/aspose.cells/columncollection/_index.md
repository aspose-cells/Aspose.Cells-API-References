---
title: ColumnCollection
second_title: Справочник по Aspose.Cells для .NET API
description: Коллекция объектов представляющих отдельные столбцы настройки на рабочем листе. Объект Column представляет только такие настройки как ширина столбца стили и т.д. для всего столбца не имеет ничего общего с тем что в соответствующем столбце есть непустые ячейки данные. И Количество этой коллекции представляет только количество объектов столбцов которые были созданы в этой коллекции не имеет ничего общего с тем фактом что есть непустые ячейки данные или нет на листе.
type: docs
weight: 1070
url: /ru/net/aspose.cells/columncollection/
---
## ColumnCollection class

Коллекция объектов, представляющих отдельные столбцы (настройки) на рабочем листе. Объект Column представляет только такие настройки, как ширина столбца, стили и т.д. для всего столбца не имеет ничего общего с тем, что в соответствующем столбце есть непустые ячейки (данные). И "Количество" этой коллекции представляет только количество объектов столбцов, которые были созданы в этой коллекции, не имеет ничего общего с тем фактом, что есть непустые ячейки (данные) или нет на листе.

```csharp
public class ColumnCollection : CollectionBase<Column>
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/columncollection/item) { get; } | Получает объектпо индексу столбца. Объект столбца с заданным индексом столбца будет создан, если он не существовал ранее. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Column) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Column, IComparer&lt;Column&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Column, IComparer&lt;Column&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Column) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Column[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Column[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Column[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Column&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Column&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Column&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Column&gt;) |  |
| [GetColumnByIndex](../../aspose.cells/columncollection/getcolumnbyindex)(int) | Получает объект[`Column`](../column)по позиции в списке. |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### Примеры

```csharp

[C#]

  //Создание экземпляра рабочей книги object
Workbook workbook = new Workbook();

//Получение ссылки на первый worksheet
Worksheet worksheet = workbook.Worksheets[0];

  //Добавить новый стиль в Workbook
Style style = workbook.CreateStyle();

  //Установка цвета фона на Blue
style.ForegroundColor = Color.Blue;

  //установка фонового рисунка
style.Pattern = BackgroundType.Solid;

  //Флаг нового стиля
StyleFlag styleFlag = new StyleFlag();

  //Установить все стили
styleFlag.All = true;

  //Изменить ширину по умолчанию для первых десяти столбцов
for (int i = 0; i < 10; i++)
{
    worksheet.Cells.Columns[i].Width = 20;
}

  //Получить столбец с нестандартным форматированием
ColumnCollection columns = worksheet.Cells.Columns;

foreach (Column column in columns)
{
      //Применяем стиль к первым десяти Columns
    column.ApplyStyle(style, styleFlag);
}

  //Сохранение файла Excel
workbook.Save("book1.xls");

[VB.NET]

'Создание экземпляра рабочей книги object
Dim workbook As Workbook = New Workbook()

'Получение ссылки на первый worksheet
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Добавить новый стиль в книгу
Dim style As Style = workbook.CreateStyles()

'Установка цвета фона на синий
style.ForegroundColor = Color.Blue

'настройка фонового рисунка
style.Pattern = BackgroundType.Solid

'Флаг нового стиля
Dim styleFlag As New StyleFlag()

'Установить все стили
styleFlag.All = True

'Изменить ширину по умолчанию первых десяти столбцов
For i As Integer = 0 To 9
    worksheet.Cells.Columns(i).Width = 20
Next i

'Получить столбец с форматированием не по умолчанию
Dim columns As ColumnCollection = worksheet.Cells.Columns

For Each column As Column In columns
    'Применить стиль к первым десяти столбцам
    column.ApplyStyle(style, styleFlag)
Next column

'Сохранение файла Excel
workbook.Save("book1.xls")

```

### Смотрите также

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [Column](../column)
* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
