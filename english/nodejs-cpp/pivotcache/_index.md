---
title: PivotCache
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the memory cache for some PivotTable reports.
type: docs
url: /nodejs-cpp/pivotcache/
---

## PivotCache class

Represents the memory cache for some PivotTable reports.

```javascript
class PivotCache;
```

### Remarks
All data will be gathered into this cache,and the pivot table only get data from this cache,not directly access data source. If data source of some [PivotTable](../pivottable/)s are same, they will use a pivot cache.

## Methods

| Method | Description |
| --- | --- |
| [refresh(PivotTableRefreshOption)](#refresh-pivottablerefreshoption-)| Refreshes data from the data source and calculates data for the view of all pivottables which data source is this pivot cache. |
| [refresh()](#refresh--)| Refreshes data from the data source and calculates data for the view of all pivottables which data source is this pivot cache. |
| [getPivotTables()](#getPivotTables--)| Gets all pivot tables with this pivot cache. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getSourceType()](#getSourceType--)| Gets the [PivotTableSourceType](../pivottablesourcetype/). |
| [dispose()](#dispose--)| Release all resource. |


### refresh(PivotTableRefreshOption) {#refresh-pivottablerefreshoption-}

Refreshes data from the data source and calculates data for the view of all pivottables which data source is this pivot cache.

```javascript
refresh(option: PivotTableRefreshOption) : PivotRefreshState;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../pivottablerefreshoption/) | The options for refreshing data source of pivot table. |

**Returns**

[PivotRefreshState](../pivotrefreshstate/)

**Remarks**

It's better that you can simply call [Workbook.RefreshAll()](../workbook.refreshall()/) to refresh all pivot tables and charts in the file.

### refresh() {#refresh--}

Refreshes data from the data source and calculates data for the view of all pivottables which data source is this pivot cache.

```javascript
refresh() : PivotRefreshState;
```


**Returns**

[PivotRefreshState](../pivotrefreshstate/)

**Remarks**

If both table1 and table2 use this cache, the two table will calculated. It's better that you can simply call [Workbook.RefreshAll()](../workbook.refreshall()/) to refresh all pivot tables and charts in the file.

### getPivotTables() {#getPivotTables--}

Gets all pivot tables with this pivot cache.

```javascript
getPivotTables() : PivotTable[];
```


**Returns**

[PivotTable](../pivottable/)[]

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### getSourceType() {#getSourceType--}

Gets the [PivotTableSourceType](../pivottablesourcetype/).

```javascript
getSourceType() : PivotTableSourceType;
```


**Returns**

[PivotTableSourceType](../pivottablesourcetype/)

### dispose() {#dispose--}

Release all resource.

```javascript
dispose() : void;
```



