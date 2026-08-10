---
title: "ConditionalFormattingCollection Class"
linktitle: "ConditionalFormattingCollection"
articleTitle: "ConditionalFormattingCollection"
second_title: "Aspose.Cells for Python via Java"
description: "Encapsulates a collection of FormatCondition objects."
type: docs
weight: 1090
url: /python-java/asposecells.api/conditionalformattingcollection/
---

## ConditionalFormattingCollection class

Encapsulates a collection of FormatCondition objects.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | int |  |
| [Item (int)](#itemint) | FormatConditionCollection | Gets the FormatConditions element at the specified index. |

## Methods

| Name | Description |
| --- | --- |
| [removeArea](#removearea) | Remove all conditional formatting in the range. |
| [copy](#copy) | Copies conditional formatting. |
| [add](#add) | Adds a FormatConditions to the collection. |
| [clear](#clear) |  |
| [removeAt](#removeat) |  |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### ConditionalFormattingCollection.Count property {#count}

**Type:** int

### ConditionalFormattingCollection.Item (int) property {#itemint}

Gets the FormatConditions element at the specified index.

**Type:** FormatConditionCollection

### removeArea(startRow, startColumn, totalRows, totalColumns) {#removearea}

Remove all conditional formatting in the range.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | The start row of the range. |
| startColumn | int | The start column of the range. |
| totalRows | int | The number of rows of the range. |
| totalColumns | int | The number of columns of the range. |

### copy(cfs) {#copy}

Copies conditional formatting.

| Parameter | Type | Description |
| --- | --- | --- |
| cfs | ConditionalFormattingCollection | The conditional formatting |

### add() (1 of 2) {#add}

Adds a FormatConditions to the collection.

**Returns:** FormatConditions object index.

---

### add(value) (2 of 2) {#add-1}

Reserved for internal use.

### clear() {#clear}

### removeAt(index) {#removeat}

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.
