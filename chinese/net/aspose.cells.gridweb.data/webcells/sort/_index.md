---
title: "WebCells.Sort"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "WebCells 方法。按指定列索引在 WebWorksheet 的范围内自上而下升序排序数据"
type: docs
url: /zh/net/aspose.cells.gridweb.data/webcells/sort/
---
## Sort(int, int, int, int, int) {#sort}

在 WebWorksheet 的范围内按指定列索引将数据从上到下升序排序。

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | Int32 | 要排序的第一个单元格的行号。 |
| startColumn | Int32 | 要排序的第一个单元格的列号。 |
| 行 | Int32 | 要导入的行数。 |
| 列 | Int32 | 要导入的列数。 |
| 索引 | Int32 | 指定排序列的列索引。 |

### 示例

```csharp

[C#]

GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,3);

[VB]

GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3)

```

### 另请参见

* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int, SortByOrder, SortOrientation, bool) {#sort_1}

在 WebWorksheet 的范围内按指定列索引将数据从上到下升序排序。

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index, 
    SortByOrder sortOrder, SortOrientation sortOrientation, bool isCaseSensitive)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | Int32 | 要排序的第一个单元格的行号。 |
| startColumn | Int32 | 要排序的第一个单元格的列号。 |
| 行 | Int32 | 要导入的行数。 |
| 列 | Int32 | 要导入的列数。 |
| 索引 | Int32 | 指定排序列（或行）的列（或行）索引。如果排序方向是自上而下，则索引表示列索引；如果排序方向是从左到右，则索引表示行索引。 |
| 顺序 | SortByOrder | 排序顺序：升序或降序 |
| 方向 | SortOrientation | 排序方向：自上而下或从左到右。 |
| isCaseSensitive | 布尔 | 指示当数据为字符串时，排序数据是否区分大小写。 |

### 示例

```csharp

[C#]

GridWeb1.WebWorksheets[0].Cells.Sort(0,1,4,14,3,SortOrder.Ascending,SortOrientation.SortLeftToRight,true)

[VB]

GridWeb1.WebWorksheets(0).Cells.Sort(0,1,4,14,3,SortOrder.Ascending,SortOrientation.SortLeftToRight,True)

```

### 另请参见

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[]) {#sort_2}

在 WebWorksheet 的范围内按列索引数组指定的字段将数据从上到下升序排序。

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | Int32 | 要排序的第一个单元格的行号。 |
| startColumn | Int32 | 要排序的第一个单元格的列号。 |
| 行 | Int32 | 要导入的行数。 |
| 列 | Int32 | 要导入的列数。 |
| 索引 | Int32[] | 指定排序依据的列索引数组。 |

### 示例

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

### 另请参见

* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) {#sort_3}

按由索引数组指定的某些字段，对 WebWorksheet 中的一个范围内的数据进行升序排序。

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes, 
    SortByOrder[] orders, SortOrientation orientation, bool isCaseSensitive)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | Int32 | 要排序的第一个单元格的行号。 |
| startColumn | Int32 | 要排序的第一个单元格的列号。 |
| 行 | Int32 | 要导入的行数。 |
| 列 | Int32 | 要导入的列数。 |
| 索引 | Int32[] | 指定排序列（或行）的列（或行）索引。如果排序方向是自上而下，则索引表示列索引；如果排序方向是从左到右，则索引表示行索引。 |
| 顺序 | SortByOrder[] | 排序顺序：升序或降序 |
| 方向 | SortOrientation | 排序方向：自上而下或从左到右。 |
| isCaseSensitive | 布尔 | 指示排序是否区分大小写。 |

### 备注

如果使用此方法对数据块进行排序，请确保参数 indexes 的长度等于参数 orders 的长度。

### 示例

```csharp

```

[C#] int[] indexes = new int[3]; indexes[0] = 0; indexes[1] = 1; indexes[2] = 3; SortOrder[] orders = new SortOrder[3]; orders[0] = SortOrder.Ascending; orders[1] = SortOrder.Descending; orders[2] = SortOrder.Descending; GridWeb1.WebWorksheets[0].Cells.Sort(0,1,4,14,indexes,orders,SortOrientation.SortLeftToRight,false); [VB] Dim indexes() As Integer = New Integer(3) {} indexes(0) = 0 indexes(1) = 1 indexes(2) = 3 Dim orders() As SortOrder = New SortOrder(3) {} orders(0) = SortOrder.Ascending orders(1) = SortOrder.Descending orders(2) = SortOrder.Descending GridWeb1.WebWorksheets(0).Cells.Sort(0,1,4,14,indexes,orders,SortOrientation.SortLeftToRight,False)

### 另请参见

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


