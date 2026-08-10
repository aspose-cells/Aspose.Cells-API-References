---
title: "DocumentPropertyCollection Class"
linktitle: "DocumentPropertyCollection"
articleTitle: "DocumentPropertyCollection"
second_title: "Aspose.Cells for Python via Java"
description: "Base class for BuiltInDocumentPropertyCollection and CustomDocumentPropertyCollection collections."
type: docs
weight: 1840
url: /python-java/asposecells.api/documentpropertycollection/
---

## DocumentPropertyCollection class

Base class for BuiltInDocumentPropertyCollection and CustomDocumentPropertyCollection collections.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | int |  |
| [Item (java.lang.String)](#itemjavalangstring) | DocumentProperty | Returns a DocumentProperty object by the name of the property. Returns null if a property with the specified name is not |
| [Item (int)](#itemint) | DocumentProperty | Returns a DocumentProperty object by index. |

## Methods

| Name | Description |
| --- | --- |
| [contains](#contains) | Returns true if a property with the specified name exists in the collection. |
| [indexOf](#indexof) | Gets the index of a property by name. |
| [remove](#remove) | Removes a property with the specified name from the collection. |
| [removeAt](#removeat) | Removes a property at the specified index. |
| [clear](#clear) |  |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [add](#add) | Reserved for internal use. |

### DocumentPropertyCollection.Count property {#count}

**Type:** int

### DocumentPropertyCollection.Item (java.lang.String) property {#itemjavalangstring}

Returns a DocumentProperty object by the name of the property. Returns null if a property with the specified name is not found.

**Type:** DocumentProperty

### DocumentPropertyCollection.Item (int) property {#itemint}

Returns a DocumentProperty object by index.

**Type:** DocumentProperty

### contains(name) (1 of 2) {#contains}

Returns true if a property with the specified name exists in the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The case-insensitive name of the property. |

**Returns:** True if the property exists in the collection; false otherwise.

---

### contains(value) (2 of 2) {#contains-1}

Reserved for internal use.

### indexOf(name) (1 of 2) {#indexof}

Gets the index of a property by name.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The case-insensitive name of the property. |

**Returns:** The zero based index. Negative value if not found.

---

### indexOf(value) (2 of 2) {#indexof-1}

Reserved for internal use.

### remove(name) {#remove}

Removes a property with the specified name from the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The case-insensitive name of the property. |

### removeAt(index) {#removeat}

Removes a property at the specified index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index. |

### clear() {#clear}

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### add(value) {#add}

Reserved for internal use.
