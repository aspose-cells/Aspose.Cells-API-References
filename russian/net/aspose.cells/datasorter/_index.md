---
title: DataSorter
second_title: Справочник по Aspose.Cells для .NET API
description: Краткое описание DataSorter.
type: docs
weight: 1300
url: /ru/net/aspose.cells/datasorter/
---
## DataSorter class

Краткое описание DataSorter.

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
| [SortAsNumber](../../aspose.cells/datasorter/sortasnumber) { get; set; } | Указывает, сортируется ли что-либо похожее на число. |
| [SortLeftToRight](../../aspose.cells/datasorter/sortlefttoright) { get; set; } | True означает, что сортировка осуществляется слева направо. False означает, что сортировка осуществляется сверху вниз. Значение по умолчанию — false. |

## Методы

| Имя | Описание |
| --- | --- |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey_1)(int, SortOrder) | Добавляет отсортированный индекс столбца и порядок сортировки. |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey_2)(int, SortOrder, string) | Добавляет отсортированный индекс столбца и порядок сортировки с пользовательским списком сортировки. |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey_3)(int, SortOrder, string[]) | Добавляет отсортированный индекс столбца и порядок сортировки с пользовательским списком сортировки. |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey)(int, SortOnType, SortOrder, object) | Добавляет отсортированный индекс столбца и порядок сортировки с пользовательским списком сортировки. |
| [Clear](../../aspose.cells/datasorter/clear)() | Сбросить все настройки. |
| [Sort](../../aspose.cells/datasorter/sort#sort)() | Сортировка данных в диапазоне. |
| [Sort](../../aspose.cells/datasorter/sort#sort_1)(Cells, CellArea) | Сортировка данных области. |
| [Sort](../../aspose.cells/datasorter/sort#sort_2)(Cells, int, int, int, int) | Сортирует данные области. |

### Примеры

```csharp

[C#]

  //Создаем новый объект Workbook.
Workbook workbook = new Workbook("Book1.xls");
  //Получить объект сортировщика данных рабочей книги.
DataSorter sorter = workbook.DataSorter;
  //Установить первый порядок для объекта сортировщика данных.
sorter.Order1 = Aspose.Cells.SortOrder.Descending;
  //Определяем первый ключ.
sorter.Key1 = 0;
  //Установить второй порядок для объекта сортировщика данных.
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
  //Сортировка данных в указанном диапазоне данных (A1:B14)
sorter.Sort(workbook.Worksheets[0].Cells, ca);
  // Сохраняем файл Excel.
workbook.Save("outBook.xls");

[Visual Basic]

'Instantiate a new Workbook object.
Dim workbook As Workbook = New Workbook("Book1.xls")
'Get the workbook datasorter object.
Dim sorter As DataSorter = workbook.DataSorter
'Set the first order for datasorter object
sorter.Order1 = Aspose.Cells.SortOrder.Descending
'Define the first key.
sorter.Key1 = 0
'Set the second order for datasorter object.
sorter.Order2 = Aspose.Cells.SortOrder.Ascending
'Define the second key.
sorter.Key2 = 1
'Create a cells area (range).
Dim ca As CellArea = New CellArea
'Specify the start row index.
ca.StartRow = 0
'Specify the start column index.
ca.StartColumn = 0
'Specify the last row index.
ca.EndRow = 13
'Specify the last column index.
ca.EndColumn = 1
'Sort the data in the specified data range (A1:B14)
sorter.Sort(workbook.Worksheets(0).Cells, ca)
'Save the excel file.
workbook.Save("outBook.xls")

```

### Смотрите также

* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
