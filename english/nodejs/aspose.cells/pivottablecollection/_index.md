---
title: "PivotTableCollection"
linktitle: "PivotTableCollection"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents the collection of all the PivotTable objects on the specified worksheet."
type: docs
weight: 2920
url: /nodejs/aspose.cells/pivottablecollection/
---

## PivotTableCollection class

Represents the collection of all the PivotTable objects on the specified worksheet.

## Methods

| Name | Description |
| --- | --- |
| [add(sourceData, destCellName, tableName)](#add) | Adds a new PivotTable cache to a PivotCaches collection. |
| [add(sourceData, destCellName, tableName, useSameSource)](#add-1) | Adds a new PivotTable cache to a PivotCaches collection. |
| [add(sourceData, row, column, tableName)](#add-2) | Adds a new PivotTable cache to a PivotCaches collection. |
| [add(sourceData, row, column, tableName, useSameSource)](#add-3) | Adds a new PivotTable cache to a PivotCaches collection. |
| [add()](#add-4) |  |
| [add()](#add-5) |  |
| [add(pivotTable, destCellName, tableName)](#add-6) | Adds a new PivotTable Object to the collection from another PivotTable. |
| [add(pivotTable, row, column, tableName)](#add-7) | Adds a new PivotTable Object to the collection from another PivotTable. |
| [add(sourceData, isAutoPage, pageFields, destCellName, tableName)](#add-8) | Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source. |
| [add(sourceData, isAutoPage, pageFields, row, column, tableName)](#add-9) | Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source. |
| [add()](#add-10) | Reserved for internal use. |
| [clear()](#clear) | Clear all pivot tables. |
| [contains()](#contains) | Reserved for internal use. |
| [dispose()](#dispose) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [get()](#get) | Gets the PivotTable report by index. |
| [get()](#get-1) | Gets the PivotTable report by pivottable's name. |
| [get()](#get-2) | Gets the PivotTable report by pivottable's position. |
| [get()](#get-3) | Reserved for internal use. |
| [getCount()](#getcount) |  |
| [indexOf()](#indexof) | Reserved for internal use. |
| [iterator()](#iterator) |  |
| [remove(pivotTable)](#remove) | Deletes the specified PivotTable and delete the PivotTable data |
| [remove(pivotTable, keepData)](#remove-1) | Deletes the specified PivotTable |
| [removeAt(index)](#removeat) | Deletes the PivotTable at the specified index and delete the PivotTable data |
| [removeAt(index, keepData)](#removeat-1) | Deletes the PivotTable at the specified index |

### add(sourceData, destCellName, tableName) {#add}

Adds a new PivotTable cache to a PivotCaches collection.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data for the new PivotTable cache. |
| destCellName | String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |

**Returns:** Number — `Number` The new added cache index.

### add(sourceData, destCellName, tableName, useSameSource) {#add-1}

Adds a new PivotTable cache to a PivotCaches collection.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data for the new PivotTable cache. |
| destCellName | String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |
| useSameSource | boolean | Indicates whether using same data source when another existing pivot table has used this data source. If the property is true, it will save memory. |

**Returns:** Number — `Number` The new added cache index.

### add(sourceData, row, column, tableName) {#add-2}

Adds a new PivotTable cache to a PivotCaches collection.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| row | Number | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | Number | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |

**Returns:** Number — `Number` The new added cache index.

### add(sourceData, row, column, tableName, useSameSource) {#add-3}

Adds a new PivotTable cache to a PivotCaches collection.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| row | Number | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | Number | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |
| useSameSource | boolean | Indicates whether using same data source when another existing pivot table has used this data source. If the property is true, it will save memory. |

**Returns:** Number — `Number` The new added cache index.

### add() {#add-4}

### add() {#add-5}

### add(pivotTable, destCellName, tableName) {#add-6}

Adds a new PivotTable Object to the collection from another PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | The source pivotTable. |
| destCellName | String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |

**Returns:** Number — `Number` The new added PivotTable index.

### add(pivotTable, row, column, tableName) {#add-7}

Adds a new PivotTable Object to the collection from another PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | The source pivotTable. |
| row | Number | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | Number | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |

**Returns:** Number — `Number` The new added PivotTable index.

### add(sourceData, isAutoPage, pageFields, destCellName, tableName) {#add-8}

Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | Array of String | The multiple consolidation ranges,such as {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | boolean | Whether auto create a single page field. If true,the following param pageFields will be ignored. |
| pageFields | PivotPageFields | The pivot page field items. |
| destCellName | String | destCellName The name of the new PivotTable report. |
| tableName | String | the name of the new PivotTable report. |

**Returns:** Number — `Number` The new added PivotTable index.

### add(sourceData, isAutoPage, pageFields, row, column, tableName) {#add-9}

Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source.

| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | Array of String | The multiple consolidation ranges,such as {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | boolean | Whether auto create a single page field. If true,the following param pageFields will be ignored |
| pageFields | PivotPageFields | The pivot page field items. |
| row | Number | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | Number | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |

**Returns:** Number — `Number` The new added PivotTable index.

### add() {#add-10}

Reserved for internal use.

### clear() {#clear}

Clear all pivot tables.

### contains() {#contains}

Reserved for internal use.

### dispose() {#dispose}

Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

### get() {#get}

Gets the PivotTable report by index.

### get() {#get-1}

Gets the PivotTable report by pivottable's name.

### get() {#get-2}

Gets the PivotTable report by pivottable's position.

### get() {#get-3}

Reserved for internal use.

### getCount() {#getcount}

### indexOf() {#indexof}

Reserved for internal use.

### iterator() {#iterator}

### remove(pivotTable) {#remove}

Deletes the specified PivotTable and delete the PivotTable data

| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | PivotTable object |

### remove(pivotTable, keepData) {#remove-1}

Deletes the specified PivotTable

| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | PivotTable object |
| keepData | boolean | Whether to keep the PivotTable data |

### removeAt(index) {#removeat}

Deletes the PivotTable at the specified index and delete the PivotTable data

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | the position index in PivotTable collection |

### removeAt(index, keepData) {#removeat-1}

Deletes the PivotTable at the specified index

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | the position index in PivotTable collection |
| keepData | boolean | Whether to keep the PivotTable data |
