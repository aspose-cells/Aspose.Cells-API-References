---
title: Add
second_title: Aspose.Cells for .NET API 参考
description: 添加一个使用数据透视表作为数据源的新切片器
type: docs
weight: 20
url: /zh/net/aspose.cells.slicers/slicercollection/add/
---
## Add(PivotTable, string, string) {#add_5}

添加一个使用数据透视表作为数据源的新切片器

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | Slicer 范围左上角的单元格。 |
| baseFieldName | String | PivotTable.BaseFields 中PivotField 的名称 |

### 返回值

新添加的切片器索引

### 例子

```csharp

[C#]

slicers.Add(pivot, "E3", "fruit");
```

### 也可以看看

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* 命名空间 [Aspose.Cells.Slicers](../../slicercollection)
* 部件 [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add_2}

添加一个使用数据透视表作为数据源的新切片器

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Int32 | Slicer 范围左上角单元格的行索引。 |
| column | Int32 | 切片器范围左上角单元格的列索引。 |
| baseFieldName | String | PivotTable.BaseFields 中PivotField 的名称 |

### 返回值

新添加的切片器索引

### 例子

```csharp

[C#]

slicers.Add(pivot, 20, 12, "fruit");
```

### 也可以看看

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* 命名空间 [Aspose.Cells.Slicers](../../slicercollection)
* 部件 [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

添加一个使用数据透视表作为数据源的新切片器

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Int32 | Slicer 范围左上角单元格的行索引。 |
| column | Int32 | 切片器范围左上角单元格的列索引。 |
| baseFieldIndex | Int32 | PivotField 在 PivotTable.BaseFields 中的索引 |

### 返回值

新添加的 Slicer 索引

### 例子

```csharp

[C#]

slicers.Add(pivot, 20, 8, 0);
```

### 也可以看看

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* 命名空间 [Aspose.Cells.Slicers](../../slicercollection)
* 部件 [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

添加一个使用数据透视表作为数据源的新切片器

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | Slicer 范围左上角的单元格。 |
| baseFieldIndex | Int32 | PivotField 在 PivotTable.BaseFields 中的索引 |

### 返回值

新添加的 Slicer 索引

### 例子

```csharp

[C#]

slicers.Add(pivot, "E20", 0);
```

### 也可以看看

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* 命名空间 [Aspose.Cells.Slicers](../../slicercollection)
* 部件 [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

添加一个使用数据透视表作为数据源的新切片器

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Int32 | Slicer 范围左上角单元格的行索引。 |
| column | Int32 | 切片器范围左上角单元格的列索引。 |
| baseField | PivotField | PivotTable.BaseFields 中的 PivotField |

### 返回值

新添加的切片器索引

### 例子

```csharp

[C#]

slicers.Add(pivot, 3, 12, pivot.BaseFields[0]);
```

### 也可以看看

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [SlicerCollection](../../slicercollection)
* 命名空间 [Aspose.Cells.Slicers](../../slicercollection)
* 部件 [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

添加一个使用数据透视表作为数据源的新切片器

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | Slicer 范围左上角的单元格。 |
| baseField | PivotField | PivotTable.BaseFields 中的 PivotField |

### 返回值

新添加的切片器索引

### 例子

```csharp

[C#]

slicers.Add(pivot, "I3", pivot.BaseFields[0]);
```

### 也可以看看

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [SlicerCollection](../../slicercollection)
* 命名空间 [Aspose.Cells.Slicers](../../slicercollection)
* 部件 [Aspose.Cells](../../../)

---

## Add(ListObject, int, string) {#add_8}

使用 ListObjet 作为数据源添加新切片器

```csharp
public int Add(ListObject table, int index, string destCellName)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| table | ListObject | ListObject object |
| index | Int32 | ListObject.ListColumns中ListColumn的索引 |
| destCellName | String | 上层单元格- 切片器范围的左角。 |

### 返回值

新添加的切片器索引

### 例子

```csharp

[C#]

slicers.Add(table, 1, "E38");
```

### 也可以看看

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [SlicerCollection](../../slicercollection)
* 命名空间 [Aspose.Cells.Slicers](../../slicercollection)
* 部件 [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, string) {#add_7}

使用 ListObjet 作为数据源添加新切片器

```csharp
public int Add(ListObject table, ListColumn listColumn, string destCellName)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| table | ListObject | ListObject object |
| listColumn | ListColumn | ListObject.ListColumns 中的 ListColumn |
| destCellName | String | 左上角的单元格切片机系列的一角。 |

### 返回值

新添加的切片器索引

### 例子

```csharp

[C#]

slicers.Add(table, table.ListColumns[1], "I38");
```

### 也可以看看

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [ListColumn](../../../aspose.cells.tables/listcolumn)
* class [SlicerCollection](../../slicercollection)
* 命名空间 [Aspose.Cells.Slicers](../../slicercollection)
* 部件 [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, int, int) {#add_6}

使用 ListObjet 作为数据源添加新切片器

```csharp
public int Add(ListObject table, ListColumn listColumn, int row, int column)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| table | ListObject | ListObject object |
| listColumn | ListColumn | ListObject.ListColumns |
| row | Int32 | 中单元格的行索引切片器范围的左上角。 |
| column | Int32 | 切片器范围左上角单元格的列索引。 |

### 返回值

新添加的切片器索引

### 例子

```csharp

[C#]

slicers.Add(table, table.ListColumns[1], 38, 12);
```

### 也可以看看

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [ListColumn](../../../aspose.cells.tables/listcolumn)
* class [SlicerCollection](../../slicercollection)
* 命名空间 [Aspose.Cells.Slicers](../../slicercollection)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
