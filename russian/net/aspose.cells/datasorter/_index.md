---
title: DataSorter
second_title: Справочник по Aspose.Cells для .NET API
description: Краткое описание для DataSorter.
type: docs
weight: 1300
url: /ru/net/aspose.cells/datasorter/
---
## DataSorter class

Краткое описание для DataSorter.

```csharp
public class DataSorter
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [CaseSensitive](../../aspose.cells/datasorter/casesensitive) { get; set; } | Получает и устанавливает, учитывается ли регистр при сравнении строки. |
| [HasHeaders](../../aspose.cells/datasorter/hasheaders) { get; set; } | Указывает, есть ли у диапазона заголовки. |
| [Key1](../../aspose.cells/datasorter/key1) { get; set; } | Представляет индекс первого отсортированного столбца (абсолютная позиция, столбец A равен 0, B равен 1, ...). |
| [Key2](../../aspose.cells/datasorter/key2) { get; set; } | Представляет индекс второго отсортированного столбца (абсолютная позиция, столбец A равен 0, B равен 1, ...). |
| [Key3](../../aspose.cells/datasorter/key3) { get; set; } | Представляет индекс третьего отсортированного столбца (абсолютная позиция, столбец A равен 0, B равен 1, ...). |
| [Keys](../../aspose.cells/datasorter/keys) { get; } | Получает список ключей сортировщика данных. |
| [Order1](../../aspose.cells/datasorter/order1) { get; set; } | Представляет порядок сортировки первого ключа. |
| [Order2](../../aspose.cells/datasorter/order2) { get; set; } | Представляет порядок сортировки второго ключа. |
| [Order3](../../aspose.cells/datasorter/order3) { get; set; } | Представляет порядок сортировки третьего ключа. |
| [SortAsNumber](../../aspose.cells/datasorter/sortasnumber) { get; set; } | Указывает, сортируется ли что-либо, похожее на число. |
| [SortLeftToRight](../../aspose.cells/datasorter/sortlefttoright) { get; set; } | True означает, что сортировка выполняется слева направо. False означает, что сортировка выполняется сверху вниз. Значение по умолчанию — false. |

## Методы

| Имя | Описание |
| --- | --- |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey_1)(int, SortOrder) | Добавляет отсортированный индекс столбца и порядок сортировки. |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey_2)(int, SortOrder, string) | Добавляет отсортированный индекс столбца и порядок сортировки с пользовательским списком сортировки. |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey_3)(int, SortOrder, string[]) | Добавляет отсортированный индекс столбца и порядок сортировки с пользовательским списком сортировки. |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey)(int, SortOnType, SortOrder, object) | Добавляет отсортированный индекс столбца и порядок сортировки с пользовательским списком сортировки. |
| [Clear](../../aspose.cells/datasorter/clear)() | Сбросить все настройки. |
| [Sort](../../aspose.cells/datasorter/sort#sort)() | Сортировать данные в диапазоне. |
| [Sort](../../aspose.cells/datasorter/sort#sort_1)(Cells, CellArea) | Сортировка данных области. |
| [Sort](../../aspose.cells/datasorter/sort#sort_2)(Cells, int, int, int, int) | Сортирует данные области. |

### Примеры

```csharp

[C#]

//Создание нового объекта Workbook.
Workbook workbook = new Workbook("Book1.xls");
//Получить объект сортировщика данных рабочей книги.
DataSorter sorter = workbook.DataSorter;
//Устанавливаем первый порядок для объекта сортировщика данных.
sorter.Order1 = Aspose.Cells.SortOrder.Descending;
//Определяем первый ключ.
sorter.Key1 = 0;
//Устанавливаем второй порядок для объекта сортировщика данных.
sorter.Order2 = Aspose.Cells.SortOrder.Ascending;
//Определяем второй ключ.
sorter.Key2 = 1;
//Создаем область ячеек (диапазон).
CellArea ca = new CellArea();
// Указываем индекс начальной строки.
ca.StartRow = 0;
// Указываем индекс начального столбца.
ca.StartColumn = 0;
// Указываем индекс последней строки.
ca.EndRow = 13;
// Указываем индекс последнего столбца.
ca.EndColumn = 1;
//Сортируем данные в указанном диапазоне данных (A1:B14)
sorter.Sort(workbook.Worksheets[0].Cells, ca);
// Сохраняем файл excel.
workbook.Save("outBook.xls");

[Visual Basic]

'Создайте новый объект Workbook.
Dim workbook As Workbook = New Workbook("Book1.xls")
'Получите объект сортировщика данных рабочей книги.
Dim sorter As DataSorter = workbook.DataSorter
'Установите первый порядок для объекта сортировщика данных
sorter.Order1 = Aspose.Cells.SortOrder.Descending
'Определите первый ключ.
sorter.Key1 = 0
'Установите второй порядок для объекта сортировщика данных.
sorter.Order2 = Aspose.Cells.SortOrder.Ascending
'Определите второй ключ.
sorter.Key2 = 1
'Создайте область ячеек (диапазон).
Dim ca As CellArea = New CellArea
'Укажите индекс начальной строки.
ca.StartRow = 0
'Укажите индекс начального столбца.
ca.StartColumn = 0
'Укажите индекс последней строки.
ca.EndRow = 13
'Укажите индекс последнего столбца.
ca.EndColumn = 1
'Сортировка данных в указанном диапазоне данных (A1:B14)
sorter.Sort(workbook.Worksheets(0).Cells, ca)
'Сохраните файл Excel.
workbook.Save("outBook.xls")

```

### Смотрите также

* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
