---
title: "GridCells.Sort"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridCells. Сортирует данные по возрастанию/убыванию сверху вниз в диапазоне листа по указанному индексу столбца. Сортирует данные по возрастанию/убыванию слева направо в диапазоне листа по указанному индексу строки"
type: docs
url: /ru/net/aspose.cells.griddesktop.data/gridcells/sort/
---
## Sort(int, int, int, int, int, bool, bool, bool) {#sort}

Сортирует данные по возрастанию/убыванию сверху вниз в диапазоне листа по указанному индексу столбца. Сортирует данные по возрастанию/убыванию слева направо в диапазоне листа по указанному индексу строки.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index, bool isAsending, 
    bool isCaseSensitive, bool islefttoright)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Номер строки первой ячейки для сортировки. |
| startColumn | Int32 | Номер столбца первой ячейки для сортировки. |
| строки | Int32 | Количество строк для импорта. |
| столбцы | Int32 | Количество столбцов для импорта. |
| индекс | Int32 | Индекс столбца, указывающий столбец сортировки. Если ориентация сверху вниз, он обозначает индекс столбца, указывающий столбец сортировки. Если ориентация слева направо, он обозначает индекс строки, указывающий строку сортировки. |
| isAsending | Boolean | является ли порядок сортировки восходящим. |
| isCaseSensitive | Boolean | является ли сортировка чувствительной к регистру. |
| islefttoright | Boolean | является ли ориентация сортировки слева направо |

### Примеры

```csharp

 [C#]

 GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,3,true,true,false);

 [VB]

 GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3,true,true,false)

```

### См. также

* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Sort(int, int, int, int, int[], SortOrder[], SortOrientation, bool) {#sort_1}

Сортирует данные области.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes, 
    SortOrder[] orders, SortOrientation orientation, bool isCaseSensitive)
```

| Параметр | Описание |
| --- | --- |
| ячейки | Ячейки содержат область данных. |
| startRow | Начальная строка области. |
| startColumn | Начальный столбец области. |
| строки | общее количество строк. |
| столбцы | Общее количество столбцов. |
| индексы | Массив отсортированных индексов столбцов |
| порядки | Массив отсортированных порядков |
| ориентация | ориентация сортировки: слева направо или сверху вниз. |
| isCaseSensitive | является ли сравнение строк чувствительным к регистру. |

### См. также

* enum [SortOrder](../../../aspose.cells.griddesktop/sortorder/)
* enum [SortOrientation](../../../aspose.cells.griddesktop/sortorientation/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


