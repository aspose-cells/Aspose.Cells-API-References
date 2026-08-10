---
title: "CollectionBase Class"
linktitle: "CollectionBase"
articleTitle: "CollectionBase"
second_title: "Aspose.Cells for Python via Java"
description: "Provides the abstract base class for a strongly typed collection."
type: docs
weight: 930
url: /python-java/asposecells.api/collectionbase/
---

## CollectionBase class

Provides the abstract base class for a strongly typed collection.

## Constructors

| Name | Description |
| --- | --- |
| [CollectionBase](#constructor) | Initializes a new instance of the CollectionBase class with the default initial capacity. |
| [CollectionBase](#constructor) | Initializes a new instance of the CollectionBase class with the specified capacity. |

## Methods

| Name | Description |
| --- | --- |
| [iterator](#iterator) | Returns an enumerator that iterates through the CollectionBase instance. |
| [getCount](#getcount) | Gets the number of elements contained in the CollectionBase instance. |
| [clear](#clear) | Removes all objects from the CollectionBase instance. |
| [add](#add) | Adds an item to the CollectionBase instance. |
| [get](#get) | Get an item at specified position. |
| [contains](#contains) | Return whether instance contains this object |
| [removeAt](#removeat) | Removes the item at the specified index. |
| [indexOf](#indexof) | Determines the index of a specific item in the CollectionBase instance. |

### CollectionBase() (1 of 2) {#constructor}

Initializes a new instance of the CollectionBase class with the default initial capacity.

---

### CollectionBase(capacity) (2 of 2) {#constructor-1}

Initializes a new instance of the CollectionBase class with the specified capacity.

| Parameter | Type | Description |
| --- | --- | --- |
| capacity | int | The number of elements that the new list can initially store. |

### iterator() {#iterator}

Returns an enumerator that iterates through the CollectionBase instance.

**Returns:** An iterator for the CollectionBase instance.

### getCount() {#getcount}

Gets the number of elements contained in the CollectionBase instance.

**Returns:** The number of elements contained in the CollectionBase instance.

### clear() {#clear}

Removes all objects from the CollectionBase instance.

### add(o) {#add}

Adds an item to the CollectionBase instance.

| Parameter | Type | Description |
| --- | --- | --- |
| o | Object | The Object to add to the CollectionBase instance. |

**Returns:** The position into which the new element was inserted.

### get(index) {#get}

Get an item at specified position.

| Parameter | Type | Description |
| --- | --- | --- |
| index | int | Specified position index. |

**Returns:** The item at specified position.

### contains(o) {#contains}

Return whether instance contains this object

| Parameter | Type | Description |
| --- | --- | --- |
| o | Object | test object |

**Returns:** Whether instance contains this object

### removeAt(index) {#removeat}

Removes the item at the specified index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero-based index of the item to remove. |

### indexOf(o) {#indexof}

Determines the index of a specific item in the CollectionBase instance.

| Parameter | Type | Description |
| --- | --- | --- |
| o | Object | Determines the index of a specific item in the CollectionBase instance. |

**Returns:** The index of value if found in the list; otherwise, -1.
