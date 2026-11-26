---
title: "GridCells.Sort"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridCells. Сортирует данные по возрастанию/убыванию сверху вниз в диапазоне листа по указанному индексу столбца. Сортирует данные по возрастанию/убыванию слева направо в диапазоне листа по указанному индексу строки"
type: docs
url: /ru/net/aspose.cells.gridweb.data/gridcells/sort/
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
 GridWeb GridWeb1 = new GridWeb();
 GridWeb1.WorkSheets[0].Cells.Sort(1,0,25,6,3,true,true,false);

 [VB]

 GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3,true,true,false)

```

### См. также

* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) {#sort_1}

Сортирует данные по возрастанию/убыванию сверху вниз в диапазоне листа по указанному индексу столбца. Сортирует данные по возрастанию/убыванию слева направо в диапазоне листа по указанному индексу строки.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes, 
    SortByOrder[] orders, SortOrientation orientation, bool isCaseSensitive)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Номер строки первой ячейки для сортировки. |
| startColumn | Int32 | Номер столбца первой ячейки для сортировки. |
| строки | Int32 | Количество строк для импорта. |
| столбцы | Int32 | Количество столбцов для импорта. |
| индексы | Int32[] | Массив индексов столбцов, указывающий столбец сортировки. Если ориентация сверху вниз, он представляет индекс столбца, определяющего сортировку. Если ориентация слева направо, он представляет индекс строки, определяющей сортировку строки. |
| порядки | SortByOrder[] | массив порядка сортировки. |
| ориентация | SortOrientation | ориентация сортировки |
| isCaseSensitive | Boolean | является ли сортировка чувствительной к регистру. |

### Примеры

```csharp

 [C#]
 GridWeb GridWeb1=new GridWeb();
 int[] ids={0,1};
 SortByOrder[] sorder={SortByOrder.Ascending,SortByOrder.Descending};
 GridWeb1.WorkSheets[0].Cells.Sort(1,0,25,6,ids,sorder,SortOrientation.SortTopToBottom,false);

 [VB]

 GridWeb1.WorkSheets(0).Cells.Sort(1,0,25,6,ids,sorder,SortOrientation.SortTopToBottom,false)

```

### См. также

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


