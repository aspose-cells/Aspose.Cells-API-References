---
title: Add
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 20
url: /net/aspose.cells.pivot/pivottablecollection/add/
---
## PivotTableCollection.Add method (1 of 8)

Adds a new PivotTable cache to a PivotCaches collection.

```csharp
public int Add(string sourceData, string destCellName, string tableName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data for the new PivotTable cache. |
| destCellName | String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |

### Return Value

The new added cache index.

### See Also

* class [PivotTableCollection](../../pivottablecollection)
* namespace [Aspose.Cells.Pivot](../../pivottablecollection)
* assembly [Aspose.Cells](../../../)

---

## PivotTableCollection.Add method (2 of 8)

Adds a new PivotTable cache to a PivotCaches collection.

```csharp
public int Add(string sourceData, string destCellName, string tableName, bool useSameSource)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data for the new PivotTable cache. |
| destCellName | String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |
| useSameSource | Boolean | Indicates whether using same data source when another existing pivot table has used this data source. If the property is true, it will save memory. |

### Return Value

The new added cache index.

### See Also

* class [PivotTableCollection](../../pivottablecollection)
* namespace [Aspose.Cells.Pivot](../../pivottablecollection)
* assembly [Aspose.Cells](../../../)

---

## PivotTableCollection.Add method (3 of 8)

Adds a new PivotTable cache to a PivotCaches collection.

```csharp
public int Add(string sourceData, int row, int column, string tableName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| row | Int32 | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | Int32 | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |

### Return Value

The new added cache index.

### See Also

* class [PivotTableCollection](../../pivottablecollection)
* namespace [Aspose.Cells.Pivot](../../pivottablecollection)
* assembly [Aspose.Cells](../../../)

---

## PivotTableCollection.Add method (4 of 8)

Adds a new PivotTable cache to a PivotCaches collection.

```csharp
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| row | Int32 | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | Int32 | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |
| useSameSource | Boolean | Indicates whether using same data source when another existing pivot table has used this data source. If the property is true, it will save memory. |

### Return Value

The new added cache index.

### See Also

* class [PivotTableCollection](../../pivottablecollection)
* namespace [Aspose.Cells.Pivot](../../pivottablecollection)
* assembly [Aspose.Cells](../../../)

---

## PivotTableCollection.Add method (5 of 8)

Adds a new PivotTable Object to the collection from another PivotTable.

```csharp
public int Add(PivotTable pivotTable, string destCellName, string tableName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | The source pivotTable. |
| destCellName | String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |

### Return Value

The new added PivotTable index.

### See Also

* class [PivotTable](../../pivottable)
* class [PivotTableCollection](../../pivottablecollection)
* namespace [Aspose.Cells.Pivot](../../pivottablecollection)
* assembly [Aspose.Cells](../../../)

---

## PivotTableCollection.Add method (6 of 8)

Adds a new PivotTable Object to the collection from another PivotTable.

```csharp
public int Add(PivotTable pivotTable, int row, int column, string tableName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | The source pivotTable. |
| row | Int32 | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | Int32 | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |

### Return Value

The new added PivotTable index.

### See Also

* class [PivotTable](../../pivottable)
* class [PivotTableCollection](../../pivottablecollection)
* namespace [Aspose.Cells.Pivot](../../pivottablecollection)
* assembly [Aspose.Cells](../../../)

---

## PivotTableCollection.Add method (7 of 8)

Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, 
    string destCellName, string tableName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String[] | The multiple consolidation ranges,such as {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | Boolean | Whether auto create a single page field. If true,the following param pageFields will be ignored. |
| pageFields | PivotPageFields | The pivot page field items. |
| destCellName | String | destCellName The name of the new PivotTable report. |
| tableName | String | the name of the new PivotTable report. |

### Return Value

The new added PivotTable index.

### See Also

* class [PivotPageFields](../../pivotpagefields)
* class [PivotTableCollection](../../pivottablecollection)
* namespace [Aspose.Cells.Pivot](../../pivottablecollection)
* assembly [Aspose.Cells](../../../)

---

## PivotTableCollection.Add method (8 of 8)

Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, int row, 
    int column, string tableName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String[] | The multiple consolidation ranges,such as {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | Boolean | Whether auto create a single page field. If true,the following param pageFields will be ignored |
| pageFields | PivotPageFields | The pivot page field items. |
| row | Int32 | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | Int32 | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |

### Return Value

The new added PivotTable index.

### See Also

* class [PivotPageFields](../../pivotpagefields)
* class [PivotTableCollection](../../pivottablecollection)
* namespace [Aspose.Cells.Pivot](../../pivottablecollection)
* assembly [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
