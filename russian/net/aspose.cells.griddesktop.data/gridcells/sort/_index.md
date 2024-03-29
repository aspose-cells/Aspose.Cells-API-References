---
title: Sort
second_title: Справочник по Aspose.Cells для .NET API
description: Сортирует данные по возрастанию/убыванию сверху вниз в диапазоне таблицы по указанному индексу столбца. Сортирует данные по возрастанию/убыванию слева направо в диапазоне таблицы по указанному индексу строки.
type: docs
weight: 690
url: /ru/net/aspose.cells.griddesktop.data/gridcells/sort/
---
## Sort(int, int, int, int, int, bool, bool, bool) {#sort}

Сортирует данные по возрастанию/убыванию сверху вниз в диапазоне таблицы по указанному индексу столбца. Сортирует данные по возрастанию/убыванию слева направо в диапазоне таблицы по указанному индексу строки.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index, bool isAsending, 
    bool isCaseSensitive, bool islefttoright)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Номер строки первой ячейки для сортировки. |
| startColumn | Int32 | Номер столбца первой ячейки для сортировки. |
| rows | Int32 | Количество строк для импорта. |
| columns | Int32 | Количество столбцов, которые необходимо импортировать. |
| index | Int32 | Индекс столбца, который определяет столбец сортировки. , если ориентация сверху вниз, он обозначает индекс столбца, который указывает столбец сортировки. , если ориентация слева направо, он обозначает индекс строки, который указывает сортировку строка. |
| isAsending | Boolean | соответствует ли порядок сортировки. |
| isCaseSensitive | Boolean | является ли сортировка регистрозависимой. |
| islefttoright | Boolean | является ли ориентация сортировки слева направо |

### Примеры

```csharp

 [C#]

 GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,3,true,true,false);

 [VB]

 GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3,true,true,false)

```

### Смотрите также

* class [GridCells](../../gridcells)
* пространство имен [Aspose.Cells.GridDesktop.Data](../../gridcells)
* сборка [Aspose.Cells.GridDesktop](../../../)

---

## Sort(int, int, int, int, int[], SortOrder[], SortOrientation, bool) {#sort_1}

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes, 
    SortOrder[] orders, SortOrientation orientation, bool isCaseSensitive)
```

### Смотрите также

* enum [SortOrder](../../../aspose.cells.griddesktop/sortorder)
* enum [SortOrientation](../../../aspose.cells.griddesktop/sortorientation)
* class [GridCells](../../gridcells)
* пространство имен [Aspose.Cells.GridDesktop.Data](../../gridcells)
* сборка [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
