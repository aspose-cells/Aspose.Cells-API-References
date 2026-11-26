---
title: "WebCells.Sort"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WebCells. Сортирует данные по возрастанию сверху вниз в диапазоне WebWorksheet по указанному индексу столбца"
type: docs
url: /ru/net/aspose.cells.gridweb.data/webcells/sort/
---
## Sort(int, int, int, int, int) {#sort}

Сортирует данные по возрастанию сверху вниз в диапазоне WebWorksheet по указанному индексу столбца.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Номер строки первой ячейки для сортировки. |
| startColumn | Int32 | Номер столбца первой ячейки для сортировки. |
| строки | Int32 | Количество строк для импорта. |
| столбцы | Int32 | Количество столбцов для импорта. |
| индекс | Int32 | Индекс столбца, указывающий столбец сортировки. |

### Примеры

```csharp

[C#]

GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,3);

[VB]

GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3)

```

### См. также

* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int, SortByOrder, SortOrientation, bool) {#sort_1}

Сортирует данные по возрастанию сверху вниз в диапазоне WebWorksheet по указанному индексу столбца.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index, 
    SortByOrder sortOrder, SortOrientation sortOrientation, bool isCaseSensitive)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Номер строки первой ячейки для сортировки. |
| startColumn | Int32 | Номер столбца первой ячейки для сортировки. |
| строки | Int32 | Количество строк для импорта. |
| столбцы | Int32 | Количество столбцов для импорта. |
| индекс | Int32 | Индекс столбца (или строки), указывающий столбец (или строку) сортировки. Если ориентация сортировки сверху вниз, индекс представляет индекс столбца. Если ориентация сортировки слева направо, индекс представляет индекс строки. |
| порядок | SortByOrder | Порядок сортировки: по возрастанию или по убыванию. |
| ориентация | SortOrientation | Ориентация сортировки: сверху вниз или слева направо. |
| isCaseSensitive | Boolean | Указывает, чувствительны ли данные сортировки к регистру, если данные являются строкой. |

### Примеры

```csharp

[C#]

GridWeb1.WebWorksheets[0].Cells.Sort(0,1,4,14,3,SortOrder.Ascending,SortOrientation.SortLeftToRight,true)

[VB]

GridWeb1.WebWorksheets(0).Cells.Sort(0,1,4,14,3,SortOrder.Ascending,SortOrientation.SortLeftToRight,True)

```

### См. также

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[]) {#sort_2}

Сортирует данные по возрастанию сверху вниз в диапазоне WebWorksheet по полям, указанным массивом индексов столбцов.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Номер строки первой ячейки для сортировки. |
| startColumn | Int32 | Номер столбца первой ячейки для сортировки. |
| строки | Int32 | Количество строк для импорта. |
| столбцы | Int32 | Количество столбцов для импорта. |
| индексы | Int32[] | Массив индексов столбцов, определяющий, по каким данным производится сортировка. |

### Примеры

```csharp

[C#]

int[] indexes = new int[3];
indexes[0] = 0;
indexes[1] = 2;
indexes[2] = 3;
GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,indexes);

[VB]

Dim indexes() As Integer =  New Integer(3) {} 
indexes(0) = 0
indexes(1) = 2
indexes(2) = 3
GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,indexes)

```

### См. также

* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) {#sort_3}

Сортирует данные по возрастанию в диапазоне WebWorksheet по полям, указанным массивом индексов.

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
| индексы | Int32[] | Индекс столбца (или строки), указывающий столбец (или строку) сортировки. Если ориентация сортировки сверху вниз, индекс представляет индекс столбца. Если ориентация сортировки слева направо, индекс представляет индекс строки. |
| порядки | SortByOrder[] | Порядок сортировки: по возрастанию или по убыванию. |
| ориентация | SortOrientation | Ориентация сортировки: сверху вниз или слева направо. |
| isCaseSensitive | Boolean | Указывает, чувствительна ли сортировка к регистру. |

### Примечания

Если вы используете этот метод для сортировки блока данных, убедитесь, что длина параметра indexes равна длине параметра orders.

### Примеры

```csharp

```

[C#] int[] indexes = new int[3]; indexes[0] = 0; indexes[1] = 1; indexes[2] = 3; SortOrder[] orders = new SortOrder[3]; orders[0] = SortOrder.Ascending; orders[1] = SortOrder.Descending; orders[2] = SortOrder.Descending; GridWeb1.WebWorksheets[0].Cells.Sort(0,1,4,14,indexes,orders,SortOrientation.SortLeftToRight,false); [VB] Dim indexes() As Integer = New Integer(3) {} indexes(0) = 0 indexes(1) = 1 indexes(2) = 3 Dim orders() As SortOrder = New SortOrder(3) {} orders(0) = SortOrder.Ascending orders(1) = SortOrder.Descending orders(2) = SortOrder.Descending GridWeb1.WebWorksheets(0).Cells.Sort(0,1,4,14,indexes,orders,SortOrientation.SortLeftToRight,False)

### См. также

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


