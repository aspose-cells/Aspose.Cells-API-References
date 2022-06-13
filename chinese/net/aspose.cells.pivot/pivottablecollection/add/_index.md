---
title: Add
second_title: Aspose.Cells for .NET API 参考
description: 将新的数据透视表缓存添加到 PivotCaches 集合
type: docs
weight: 20
url: /zh/net/aspose.cells.pivot/pivottablecollection/add/
---
## Add(string, string, string) {#add_4}

将新的数据透视表缓存添加到 PivotCaches 集合。

```csharp
public int Add(string sourceData, string destCellName, string tableName)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| sourceData | String | 新数据透视表缓存的数据。 |
| destCellName | String | 数据透视表目标区域左上角的单元格。 |
| tableName | String | 新数据透视表的名称。 |

### 返回值

新添加的缓存索引。

### 也可以看看

* class [PivotTableCollection](../../pivottablecollection)
* 命名空间 [Aspose.Cells.Pivot](../../pivottablecollection)
* 部件 [Aspose.Cells](../../../)

---

## Add(string, string, string, bool) {#add_5}

将新的数据透视表缓存添加到 PivotCaches 集合。

```csharp
public int Add(string sourceData, string destCellName, string tableName, bool useSameSource)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| sourceData | String | 新数据透视表缓存的数据。 |
| destCellName | String | 数据透视表目标区域左上角的单元格。 |
| tableName | String | 新数据透视表的名称。 |
| useSameSource | Boolean | 指示当另一个现有数据透视表已使用该数据源时是否使用相同数据源。 如果该属性为真，则会节省内存。 |

### 返回值

新添加的缓存索引。

### 也可以看看

* class [PivotTableCollection](../../pivottablecollection)
* 命名空间 [Aspose.Cells.Pivot](../../pivottablecollection)
* 部件 [Aspose.Cells](../../../)

---

## Add(string, int, int, string) {#add_2}

将新的数据透视表缓存添加到 PivotCaches 集合。

```csharp
public int Add(string sourceData, int row, int column, string tableName)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| sourceData | String | 新数据透视表的数据单元格范围。示例:Sheet1!A1:C8 |
| row | Int32 | 数据透视表目标区域左上角单元格的行索引。 |
| column | Int32 | 数据透视表目标区域左上角单元格的列索引。 |
| tableName | String | 新数据透视表的名称。 |

### 返回值

新添加的缓存索引。

### 也可以看看

* class [PivotTableCollection](../../pivottablecollection)
* 命名空间 [Aspose.Cells.Pivot](../../pivottablecollection)
* 部件 [Aspose.Cells](../../../)

---

## Add(string, int, int, string, bool) {#add_3}

将新的数据透视表缓存添加到 PivotCaches 集合。

```csharp
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| sourceData | String | 新数据透视表的数据单元格范围。示例:Sheet1!A1:C8 |
| row | Int32 | 数据透视表目标区域左上角单元格的行索引。 |
| column | Int32 | 数据透视表目标区域左上角单元格的列索引。 |
| tableName | String | 新数据透视表的名称。 |
| useSameSource | Boolean | 指示当另一个现有数据透视表已使用该数据源时是否使用相同数据源。 如果该属性为真，则会节省内存。 |

### 返回值

新添加的缓存索引。

### 也可以看看

* class [PivotTableCollection](../../pivottablecollection)
* 命名空间 [Aspose.Cells.Pivot](../../pivottablecollection)
* 部件 [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_1}

将新的数据透视表对象从另一个数据透视表添加到集合中。

```csharp
public int Add(PivotTable pivotTable, string destCellName, string tableName)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| pivotTable | PivotTable | 源数据透视表。 |
| destCellName | String | 数据透视表目标区域左上角的单元格。 |
| tableName | String | 新数据透视表的名称。 |

### 返回值

新添加的数据透视表索引。

### 也可以看看

* class [PivotTable](../../pivottable)
* class [PivotTableCollection](../../pivottablecollection)
* 命名空间 [Aspose.Cells.Pivot](../../pivottablecollection)
* 部件 [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add}

将新的数据透视表对象从另一个数据透视表添加到集合中。

```csharp
public int Add(PivotTable pivotTable, int row, int column, string tableName)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| pivotTable | PivotTable | 源数据透视表。 |
| row | Int32 | 数据透视表目标区域左上角单元格的行索引。 |
| column | Int32 | 数据透视表目标区域左上角单元格的列索引。 |
| tableName | String | 新数据透视表的名称。 |

### 返回值

新添加的数据透视表索引。

### 也可以看看

* class [PivotTable](../../pivottable)
* class [PivotTableCollection](../../pivottablecollection)
* 命名空间 [Aspose.Cells.Pivot](../../pivottablecollection)
* 部件 [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, string, string) {#add_7}

将一个新的数据透视表对象添加到具有多个合并范围作为数据源的集合中。

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, 
    string destCellName, string tableName)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| sourceData | String[] | 多个合并范围，例如 {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | Boolean | 是否自动创建单页字段。 如果为真，则以下参数 pageFields 将被忽略。 |
| pageFields | PivotPageFields | 透视页面字段项。 |
| destCellName | String | destCellName 新数据透视表的名称。 |
| tableName | String | 新数据透视表的名称。 |

### 返回值

新添加的数据透视表索引。

### 也可以看看

* class [PivotPageFields](../../pivotpagefields)
* class [PivotTableCollection](../../pivottablecollection)
* 命名空间 [Aspose.Cells.Pivot](../../pivottablecollection)
* 部件 [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, int, int, string) {#add_6}

将一个新的数据透视表对象添加到具有多个合并范围作为数据源的集合中。

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, int row, 
    int column, string tableName)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| sourceData | String[] | 多个合并范围，例如 {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | Boolean | 是否自动创建单页字段。 如果为真，以下参数 pageFields 将被忽略 |
| pageFields | PivotPageFields | 透视页面字段项。 |
| row | Int32 | 数据透视表目标区域左上角单元格的行索引。 |
| column | Int32 | 数据透视表目标区域左上角单元格的列索引。 |
| tableName | String | 新数据透视表的名称。 |

### 返回值

新添加的数据透视表索引。

### 也可以看看

* class [PivotPageFields](../../pivotpagefields)
* class [PivotTableCollection](../../pivottablecollection)
* 命名空间 [Aspose.Cells.Pivot](../../pivottablecollection)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
