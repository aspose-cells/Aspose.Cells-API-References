---
title: "PivotFieldCollection Class"
linktitle: "PivotFieldCollection"
articleTitle: "PivotFieldCollection"
second_title: "Aspose.Cells for Python via Java"
description: "Represents a collection of all the PivotField objects in the PivotTable's specific PivotFields type."
type: docs
weight: 4570
url: /python-java/asposecells.api/pivotfieldcollection/
---

## PivotFieldCollection class

Represents a collection of all the PivotField objects in the PivotTable's specific PivotFields type.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Type](#type) | int | Gets the PivotFields type. The value of the property is PivotFieldType integer constant. |
| [Count](#count) | int | Gets the count of the pivotFields. |
| [Item (int)](#itemint) | PivotField | Gets the PivotField Object at the specific index. |
| [Item (java.lang.String)](#itemjavalangstring) | PivotField | Gets the PivotField Object of the specific name. |

## Methods

| Name | Description |
| --- | --- |
| [iterator](#iterator) | Gets an enumerator over the elements in this collection in proper sequence. |
| [addByBaseIndex](#addbybaseindex) | Adds a PivotField Object to the specific type PivotFields. |
| [add](#add) | Adds a PivotField Object to the specific type PivotFields. |
| [clear](#clear) | clear all fields of PivotFieldCollection |
| [move](#move) | Moves the PivotField from current position to destination position |

### PivotFieldCollection.Type property {#type}

Gets the PivotFields type. The value of the property is PivotFieldType integer constant.

**Type:** int

### PivotFieldCollection.Count property {#count}

Gets the count of the pivotFields.

**Type:** int

### PivotFieldCollection.Item (int) property {#itemint}

Gets the PivotField Object at the specific index.

**Type:** PivotField

### PivotFieldCollection.Item (java.lang.String) property {#itemjavalangstring}

Gets the PivotField Object of the specific name.

**Type:** PivotField

### iterator() {#iterator}

Gets an enumerator over the elements in this collection in proper sequence.

**Returns:** enumerator

### addByBaseIndex(baseFieldIndex) {#addbybaseindex}

Adds a PivotField Object to the specific type PivotFields.

| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | int | field index in the base PivotFields. |

**Returns:** the index of the PivotField Object in this PivotFields.

### add(pivotField) {#add}

Adds a PivotField Object to the specific type PivotFields.

| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | PivotField | a PivotField Object. |

**Returns:** the index of the PivotField Object in this PivotFields.

### clear() {#clear}

clear all fields of PivotFieldCollection

### move(currPos, destPos) {#move}

Moves the PivotField from current position to destination position

| Parameter | Type | Description |
| --- | --- | --- |
| currPos | int | Current position of PivotField based on zero |
| destPos | int | Destination position of PivotField based on zero |
