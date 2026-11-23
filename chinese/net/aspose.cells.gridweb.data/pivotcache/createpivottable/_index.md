---
title: "PivotCache.CreatePivotTable"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotCache 方法。创建 PivotTable 报表到新 Sheet"
type: docs
url: /zh/net/aspose.cells.gridweb.data/pivotcache/createpivottable/
---
## CreatePivotTable() {#createpivottable}

在新工作表中创建 PivotTable 报表。

```csharp
public PivotTable CreatePivotTable()
```

### 返回值

PivotTable 对象

### 备注

调用此方法将创建一个 PivotTable 对象和一个新工作表。然后将该 PivotTable 对象添加到 GridWeb.Worksheets.PivotTables 的最后位置。如果调用 PivotTable.DataBind() 方法，PivotTable 报表将绘制到已创建的工作表中。

### 另请参见

* class [PivotTable](../../pivottable/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(string) {#createpivottable_3}

在新工作表中创建 PivotTable 报表。pivotTable 对象的名称

```csharp
public PivotTable CreatePivotTable(string tableName)
```

### 返回值

PivotTable 对象

### 备注

调用此方法将创建一个 PivotTable 对象和一个新工作表。然后将该 PivotTable 对象添加到 GridWeb.Worksheets.PivotTables 的最后位置。如果调用 PivotTable.DataBind() 方法，PivotTable 报表将绘制到已创建的工作表中。

### 另请参见

* class [PivotTable](../../pivottable/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(WebWorksheet, WebCell) {#createpivottable_1}

在 targetSheet 中创建 PivotTable 报表。

```csharp
public PivotTable CreatePivotTable(WebWorksheet targetSheet, WebCell targetCell)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| targetSheet | WebWorksheet | pivotTable 报表将绘制到的工作表 |
| targetCell | WebCell | pivotTable 报表将绘制到的起始单元格 |

### 返回值

PivotTable 对象

### 备注

调用此方法将创建一个 PivotTable 对象，然后将该对象添加到 GridWeb.Worksheets.PivotTables 的最后位置。如果调用 PivotTable.DataBind() 方法，PivotTable 报表将绘制到 targetSheet，并从 targetCell 开始。

### 另请参见

* class [PivotTable](../../pivottable/)
* class [WebWorksheet](../../webworksheet/)
* class [WebCell](../../webcell/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(WebWorksheet, WebCell, string) {#createpivottable_2}

在 targetSheet 中创建 PivotTable 报表。

```csharp
public PivotTable CreatePivotTable(WebWorksheet targetSheet, WebCell targetCell, string tableName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| targetSheet | WebWorksheet | pivotTable 报表将绘制到的工作表 |
| targetCell | WebCell | pivotTable 报表将绘制到的起始单元格 |
| tableName | String | pivotTable 对象的名称 |

### 返回值

PivotTable 对象

### 备注

调用此方法将创建一个名为 tableName 的 PivotTable 对象，然后将该对象添加到 GridWeb.Worksheets.PivotTables 的最后位置。如果调用 PivotTable.DataBind() 方法，PivotTable 报表将绘制到 targetSheet，并从 targetCell 开始。

### 另请参见

* class [PivotTable](../../pivottable/)
* class [WebWorksheet](../../webworksheet/)
* class [WebCell](../../webcell/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


