---
title: ConditionalFormattingIconCollection
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет набор объектовConditionalFormattingIcon./conditionalformattingicon.
type: docs
weight: 1120
url: /ru/net/aspose.cells/conditionalformattingiconcollection/
---
## ConditionalFormattingIconCollection class

Представляет набор объектов[`ConditionalFormattingIcon`](../conditionalformattingicon).

```csharp
public class ConditionalFormattingIconCollection : CollectionBase<ConditionalFormattingIcon>
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/conditionalformattingiconcollection/item) { get; } | Получает элемент ConditionalFormattingIcon по указанному индексу. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells/conditionalformattingiconcollection/add#add)(ConditionalFormattingIcon) | Добавляет[`ConditionalFormattingIcon`](../conditionalformattingicon)объект. |
| [Add](../../aspose.cells/conditionalformattingiconcollection/add#add_1)(IconSetType, int) | Добавляет[`ConditionalFormattingIcon`](../conditionalformattingicon)объект. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(ConditionalFormattingIcon) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(ConditionalFormattingIcon, IComparer&lt;ConditionalFormattingIcon&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, ConditionalFormattingIcon, IComparer&lt;ConditionalFormattingIcon&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(ConditionalFormattingIcon) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(ConditionalFormattingIcon[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(ConditionalFormattingIcon[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, ConditionalFormattingIcon[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(ConditionalFormattingIcon) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(ConditionalFormattingIcon, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(ConditionalFormattingIcon, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(ConditionalFormattingIcon) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(ConditionalFormattingIcon, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(ConditionalFormattingIcon, int, int) |  |
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

   //Устанавливает условие
 int idx = fcs.AddCondition(FormatConditionType.IconSet);
 
 FormatCondition cond = fcs[idx];
   
    //Устанавливает тип условия
 cond.IconSet.Type = IconSetType.ArrowsGray3;

  //Добавить пользовательское условие набора иконок.
 ConditionalFormattingIcon cfIcon = cond.IconSet.CfIcons[0];
 
 cfIcon.Type = IconSetType.Arrows3;
 
 cfIcon.Index = 0;
 
 ConditionalFormattingIcon cfIcon1 = cond.IconSet.CfIcons[1];
 
  cfIcon1.Type = IconSetType.ArrowsGray3;
  
  cfIcon1.Index = 1;
  
  ConditionalFormattingIcon cfIcon2 = cond.IconSet.CfIcons[2];
  
  cfIcon2.Type = IconSetType.Boxes5;
  
  cfIcon2.Index = 2;

  //Сохранение файла Excel
workbook.Save("output.xls");

[VB.NET]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()

Dim sheet As Worksheet = workbook.Worksheets(0)

'Get Conditional Formatting
Dim cformattings As ConditionalFormattingCollection = sheet.ConditionalFormattings

'Adds an empty conditional formatting
Dim index As Integer = cformattings.Add()

'Get newly added Conditional formatting
Dim fcs As FormatConditionCollection = cformattings(index)

'Sets the conditional format range.
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

   //Устанавливает условие
Dim idx As Integer =fcs.AddCondition(FormatConditionType.IconSet)

Dim cond As FormatCondition=fcs[idx]

   //Устанавливает тип условия
cfIcon.Type = IconSetType.ArrowsGray3

'Add custom iconset  condition.
Dim cfIcon As ConditionalFormattingIcon = cond.IconSet.CfIcons[0]

cfIcon.Type = IconSetType.Arrows3

cfIcon.Index=0

Dim cfIcon1 As ConditionalFormattingIcon = cond.IconSet.CfIcons[1]

cfIcon1.Type = IconSetType.ArrowsGray3

cfIcon1.Index=1

Dim cfIcon2 As ConditionalFormattingIcon = cond.IconSet.CfIcons[2]

cfIcon2.Type = IconSetType.Boxes5

cfIcon2.Index=2

'Saving the Excel file
workbook.Save("output.xls")
```

### Смотрите также

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [ConditionalFormattingIcon](../conditionalformattingicon)
* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
