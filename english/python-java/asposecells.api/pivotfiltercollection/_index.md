---
title: "PivotFilterCollection Class"
linktitle: "PivotFilterCollection"
articleTitle: "PivotFilterCollection"
second_title: "Aspose.Cells for Python via Java"
description: "Represents a collection of all the PivotFilter objects"
type: docs
weight: 4650
url: /python-java/asposecells.api/pivotfiltercollection/
---

## PivotFilterCollection class

Represents a collection of all the PivotFilter objects

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | int |  |
| [Item (int)](#itemint) | PivotFilter | Gets the pivotfilter object at the specific index. |

## Methods

| Name | Description |
| --- | --- |
| [add](#add) | Adds a PivotFilter Object to the specific type |
| [addTop10Filter](#addtop10filter) |  |
| [addValueFilter](#addvaluefilter) |  |
| [addLabelFilter](#addlabelfilter) |  |
| [addDateFilter](#adddatefilter) |  |
| [clearFilter](#clearfilter) | Clear PivotFilter from the specific PivotField |
| [clear](#clear) |  |
| [removeAt](#removeat) |  |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### PivotFilterCollection.Count property {#count}

**Type:** int

### PivotFilterCollection.Item (int) property {#itemint}

Gets the pivotfilter object at the specific index.

**Type:** PivotFilter

### add(fieldIndex, type) (1 of 2) {#add}

Adds a PivotFilter Object to the specific type

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | the PivotField index |
| type | int | A PivotFilterType value. the PivotFilter type |

**Returns:** the index of the PivotFilter Object in this PivotFilterCollection.

---

### add(value) (2 of 2) {#add-1}

Reserved for internal use.

### addTop10Filter(baseFieldIndex, valueFieldIndex, type, isTop, itemCount) {#addtop10filter}

### addValueFilter(baseFieldIndex, valueFieldIndex, type, value1, value2) {#addvaluefilter}

### addLabelFilter(baseFieldIndex, type, label1, label2) {#addlabelfilter}

### addDateFilter(baseFieldIndex, type, dateTime1, dateTime2) {#adddatefilter}

### clearFilter(fieldIndex) {#clearfilter}

Clear PivotFilter from the specific PivotField

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | int | the PivotField index |

### clear() {#clear}

### removeAt(index) {#removeat}

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.
