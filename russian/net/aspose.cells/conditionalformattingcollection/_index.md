---
title: ConditionalFormattingCollection
second_title: Справочник по Aspose.Cells для .NET API
description: Инкапсулирует коллекцию объектовFormatCondition./formatcondition.
type: docs
weight: 1100
url: /ru/net/aspose.cells/conditionalformattingcollection/
---
## ConditionalFormattingCollection class

Инкапсулирует коллекцию объектов[`FormatCondition`](../formatcondition).

```csharp
public class ConditionalFormattingCollection : CollectionBase<FormatConditionCollection>
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/conditionalformattingcollection/item) { get; } | Получает элемент FormatConditions по указанному индексу. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells/conditionalformattingcollection/add)() | Добавляет FormatConditions в коллекцию. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(FormatConditionCollection) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(FormatConditionCollection, IComparer&lt;FormatConditionCollection&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, FormatConditionCollection, IComparer&lt;FormatConditionCollection&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(FormatConditionCollection) |  |
| [Copy](../../aspose.cells/conditionalformattingcollection/copy)(ConditionalFormattingCollection) | Копирует условное форматирование. |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(FormatConditionCollection[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(FormatConditionCollection[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, FormatConditionCollection[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(FormatConditionCollection) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(FormatConditionCollection, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(FormatConditionCollection, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(FormatConditionCollection) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(FormatConditionCollection, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(FormatConditionCollection, int, int) |  |
| [RemoveArea](../../aspose.cells/conditionalformattingcollection/removearea)(int, int, int, int) | Удалить все условное форматирование в диапазоне. |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### Примеры

```csharp

[C#]

  //Создание экземпляра рабочей книги object
Workbook workbook = new Workbook();

Worksheet sheet = workbook.Worksheets[0];

//Получить условное форматирование
ConditionalFormattingCollection cformattings = sheet.ConditionalFormattings;

  //Добавляет пустое условное форматирование
int index = cformattings.Add();

  //Получить недавно добавленное условное форматирование
FormatConditionCollection fcs = cformattings[index];

  //Устанавливает диапазон условного формата.
CellArea ca = new CellArea();

ca.StartRow = 0;

ca.EndRow = 0;

ca.StartColumn = 0;

ca.EndColumn = 0;

fcs.AddArea(ca);

ca = new CellArea();

ca.StartRow = 1;

ca.EndRow = 1;

ca.StartColumn = 1;

ca.EndColumn = 1;

fcs.AddArea(ca);

   //Добавить условие.
int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");

   //Добавить условие.
int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");

  //Устанавливает цвет фона.
FormatCondition fc = fcs[conditionIndex];

fc.Style.BackgroundColor = Color.Red;

  //Сохранение файла Excel
workbook.Save("output.xls");

[VB.NET]

'Создание экземпляра рабочей книги object
DDim workbook As Workbook = New Workbook()

Dim sheet As Worksheet = workbook.Worksheets(0)

'Получить условное форматирование
Dim cformattings As ConditionalFormattingCollection = sheet.ConditionalFormattings

'Добавляет пустое условное форматирование
Dim index As Integer = cformattings.Add()

'Получить недавно добавленное условное форматирование
Dim fcs As FormatConditionCollection = cformattings(index)

'Устанавливает диапазон условного формата.
Dim ca As New CellArea()

ca.StartRow = 0

ca.EndRow = 0

ca.StartColumn = 0

ca.EndColumn = 0

fcs.AddArea(ca)

ca = New CellArea()

ca.StartRow = 1

ca.EndRow = 1

ca.StartColumn = 1

ca.EndColumn = 1

fcs.AddArea(ca)

'Добавить условие.
Dim conditionIndex As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100")

'Добавить условие.
Dim conditionIndex2 As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100")

'Устанавливает цвет фона.
Dim fc As FormatCondition = fcs(conditionIndex)

fc.Style.BackgroundColor = Color.Red

'Сохранение файла Excel
workbook.Save("output.xls")
```

### Смотрите также

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [FormatConditionCollection](../formatconditioncollection)
* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
