---
title: "PivotTableCollection Class"
linktitle: "PivotTableCollection"
articleTitle: "PivotTableCollection"
second_title: "Aspose.Cells for Python via Java"
description: "Represents the collection of all the PivotTable objects on the specified worksheet."
type: docs
weight: 4850
url: /python-java/asposecells.api/pivottablecollection/
---

## PivotTableCollection class

Represents the collection of all the PivotTable objects on the specified worksheet.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | int |  |
| [Item (int)](#itemint) | PivotTable | Gets the PivotTable report by index. |
| [Item (java.lang.String)](#itemjavalangstring) | PivotTable | Gets the PivotTable report by pivottable's name. |
| [Item (int, int)](#itemintint) | PivotTable | Gets the PivotTable report by pivottable's position. |

## Methods

| Name | Description |
| --- | --- |
| [dispose](#dispose) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [add](#add) | Adds a new PivotTable cache to a PivotCaches collection. |
| [clear](#clear) | Clear all pivot tables. |
| [remove](#remove) | Deletes the specified PivotTable and delete the PivotTable data |
| [removeAt](#removeat) | Deletes the PivotTable at the specified index and delete the PivotTable data |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### PivotTableCollection.Count property {#count}

**Type:** int

### PivotTableCollection.Item (int) property {#itemint}

Gets the PivotTable report by index.

**Type:** PivotTable

### PivotTableCollection.Item (java.lang.String) property {#itemjavalangstring}

Gets the PivotTable report by pivottable's name.

**Type:** PivotTable

### PivotTableCollection.Item (int, int) property {#itemintint}

Gets the PivotTable report by pivottable's position.

**Type:** PivotTable

### dispose() {#dispose}

Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

### add(sourceData, destCellName, tableName) (1 of 11) {#add}

Adds a new PivotTable cache to a PivotCaches collection.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data for the new PivotTable cache. |
| destCellName | String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |

**Returns:** The new added cache index.

---

### add(sourceData, destCellName, tableName, useSameSource) (2 of 11) {#add-1}

Adds a new PivotTable cache to a PivotCaches collection.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data for the new PivotTable cache. |
| destCellName | String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |
| useSameSource | boolean | Indicates whether using same data source when another existing pivot table has used this data source. If the property is true, it will save memory. |

**Returns:** The new added cache index.

---

### add(sourceData, row, column, tableName) (3 of 11) {#add-2}

Adds a new PivotTable cache to a PivotCaches collection.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| row | int | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | int | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |

**Returns:** The new added cache index.

---

### add(sourceData, row, column, tableName, useSameSource) (4 of 11) {#add-3}

Adds a new PivotTable cache to a PivotCaches collection.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| row | int | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | int | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |
| useSameSource | boolean | Indicates whether using same data source when another existing pivot table has used this data source. If the property is true, it will save memory. |

**Returns:** The new added cache index.

---

### add(sourceData, row, column, tableName, useSameSource, isXlsClassic) (5 of 11) {#add-4}

---

### add(sourceData, cell, tableName, useSameSource, isXlsClassic) (6 of 11) {#add-5}

---

### add(pivotTable, destCellName, tableName) (7 of 11) {#add-6}

Adds a new PivotTable Object to the collection from another PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | The source pivotTable. |
| destCellName | String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |

**Returns:** The new added PivotTable index.

---

### add(pivotTable, row, column, tableName) (8 of 11) {#add-7}

Adds a new PivotTable Object to the collection from another PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | The source pivotTable. |
| row | int | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | int | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |

**Returns:** The new added PivotTable index.

---

### add(sourceData, isAutoPage, pageFields, destCellName, tableName) (9 of 11) {#add-8}

Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String[] | The multiple consolidation ranges,such as {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | boolean | Whether auto create a single page field. If true,the following param pageFields will be ignored. |
| pageFields | PivotPageFields | The pivot page field items. |
| destCellName | String | destCellName The name of the new PivotTable report. |
| tableName | String | the name of the new PivotTable report. |

**Returns:** The new added PivotTable index.

---

### add(sourceData, isAutoPage, pageFields, row, column, tableName) (10 of 11) {#add-9}

Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String[] | The multiple consolidation ranges,such as {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | boolean | Whether auto create a single page field. If true,the following param pageFields will be ignored |
| pageFields | PivotPageFields | The pivot page field items. |
| row | int | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | int | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |

**Returns:** The new added PivotTable index.

---

### add(value) (11 of 11) {#add-10}

Reserved for internal use.

### clear() {#clear}

Clear all pivot tables.

### remove(pivotTable) (1 of 2) {#remove}

Deletes the specified PivotTable and delete the PivotTable data

| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | PivotTable object |

---

### remove(pivotTable, keepData) (2 of 2) {#remove-1}

Deletes the specified PivotTable

| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | PivotTable object |
| keepData | boolean | Whether to keep the PivotTable data |

### removeAt(index) (1 of 2) {#removeat}

Deletes the PivotTable at the specified index and delete the PivotTable data

| Parameter | Type | Description |
| --- | --- | --- |
| index | int | the position index in PivotTable collection |

---

### removeAt(index, keepData) (2 of 2) {#removeat-1}

Deletes the PivotTable at the specified index

| Parameter | Type | Description |
| --- | --- | --- |
| index | int | the position index in PivotTable collection |
| keepData | boolean | Whether to keep the PivotTable data |

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.
