---
title: "TableStyleCollection Class"
linktitle: "TableStyleCollection"
articleTitle: "TableStyleCollection"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents all custom table styles."
type: docs
weight: 6530
url: /php/aspose.cells/tablestylecollection/
---

## TableStyleCollection class

Represents all custom table styles.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [DefaultTableStyleName](#defaulttablestylename) | String | Gets and sets the default style name of the table. |
| [DefaultPivotStyleName](#defaultpivotstylename) | String | Gets and sets the default style name of pivot table . |
| [Count](#count) | Number |  |
| [Item (int)](#itemint) | TableStyle | Gets the table style by the index. |
| [Item (java.lang.String)](#itemjavalangstring) | TableStyle | Gets the table style by the name. |

## Methods

| Name | Description |
| --- | --- |
| [addTableStyle](#addtablestyle) | Adds a custom table style. |
| [addPivotTableStyle](#addpivottablestyle) | Adds a custom pivot table style. |
| [getBuiltinTableStyle](#getbuiltintablestyle) | Gets the builtin table style |
| [clear](#clear) |  |
| [removeAt](#removeat) |  |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [add](#add) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### TableStyleCollection.DefaultTableStyleName property {#defaulttablestylename}

Gets and sets the default style name of the table.

**Type:** String

### TableStyleCollection.DefaultPivotStyleName property {#defaultpivotstylename}

Gets and sets the default style name of pivot table .

**Type:** String

### TableStyleCollection.Count property {#count}

**Type:** Number

### TableStyleCollection.Item (int) property {#itemint}

Gets the table style by the index.

**Type:** TableStyle

### TableStyleCollection.Item (java.lang.String) property {#itemjavalangstring}

Gets the table style by the name.

**Type:** TableStyle

### addTableStyle(name) {#addtablestyle}

Adds a custom table style.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The table style name. |

**Returns:** The index of the table style.

### addPivotTableStyle(name) {#addpivottablestyle}

Adds a custom pivot table style.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The pivot table style name. |

**Returns:** The index of the pivot table style.

### getBuiltinTableStyle(type) {#getbuiltintablestyle}

Gets the builtin table style

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | A TableStyleType value. The builtin table style type. |

### clear() {#clear}

### removeAt(index) {#removeat}

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### add(value) {#add}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.
