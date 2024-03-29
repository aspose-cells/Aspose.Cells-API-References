---
title: Add
second_title: Aspose.Cells for .NET API 参考
description: 将工作表添加到集合中
type: docs
weight: 170
url: /zh/net/aspose.cells/worksheetcollection/add/
---
## Add(SheetType) {#add_2}

将工作表添加到集合中。

```csharp
public int Add(SheetType type)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| type | SheetType | 工作表类型。 |

### 返回值

[`Worksheet`](../../worksheet)对象索引。

### 例子

```csharp
[C#]
Workbook workbook = new Workbook();
workbook.Worksheets.Add(SheetType.Chart);
Cells cells = workbook.Worksheets[0].Cells;
cells["c2"].PutValue(5000);
cells["c3"].PutValue(3000);
cells["c4"].PutValue(4000);
cells["c5"].PutValue(5000);
cells["c6"].PutValue(6000);
ChartCollection charts = workbook.Worksheets[1].Charts;
int chartIndex = charts.Add(ChartType.Column, 10,10,20,20);
Chart chart = charts[chartIndex];
chart.NSeries.Add("Sheet1!C2:C6", true);

[Visual Basic]
Dim workbook As Workbook =  New Workbook() 
workbook.Worksheets.Add(SheetType.Chart)
Dim cells As Cells = workbook.Worksheets(0).Cells 
cells("c2").PutValue(5000)
cells("c3").PutValue(3000)
cells("c4").PutValue(4000)
cells("c5").PutValue(5000)
cells("c6").PutValue(6000)
Dim charts As ChartCollection = workbook.Worksheets(1).Charts
Dim chartIndex As Integer = charts.Add(ChartType.Column,10,10,20,20) 
Dim chart As Chart = charts(chartIndex) 
chart.NSeries.Add("Sheet1!C2:C6", True)
```

### 也可以看看

* enum [SheetType](../../sheettype)
* class [WorksheetCollection](../../worksheetcollection)
* 命名空间 [Aspose.Cells](../../worksheetcollection)
* 部件 [Aspose.Cells](../../../)

---

## Add() {#add_1}

将工作表添加到集合中。

```csharp
public int Add()
```

### 返回值

[`Worksheet`](../../worksheet)对象索引。

### 也可以看看

* class [WorksheetCollection](../../worksheetcollection)
* 命名空间 [Aspose.Cells](../../worksheetcollection)
* 部件 [Aspose.Cells](../../../)

---

## Add(string) {#add}

将工作表添加到集合中。

```csharp
public Worksheet Add(string sheetName)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| sheetName | String | 工作表名称 |

### 返回值

[`Worksheet`](../../worksheet)目的。

### 也可以看看

* class [Worksheet](../../worksheet)
* class [WorksheetCollection](../../worksheetcollection)
* 命名空间 [Aspose.Cells](../../worksheetcollection)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
