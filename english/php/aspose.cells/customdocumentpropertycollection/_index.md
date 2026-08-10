---
title: "CustomDocumentPropertyCollection Class"
linktitle: "CustomDocumentPropertyCollection"
articleTitle: "CustomDocumentPropertyCollection"
second_title: "Aspose.Cells for PHP via Java"
description: "A collection of custom document properties."
type: docs
weight: 1380
url: /php/aspose.cells/customdocumentpropertycollection/
---

## CustomDocumentPropertyCollection class

A collection of custom document properties.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | Number |  |
| [Item (java.lang.String)](#itemjavalangstring) | DocumentProperty | Returns a DocumentProperty object by the name of the property. Returns null if a property with the specified name is not |
| [Item (int)](#itemint) | DocumentProperty | Returns a DocumentProperty object by index. |

## Methods

| Name | Description |
| --- | --- |
| [add](#add) | Creates a new custom document property of the PropertyType.String data type. |
| [addLinkToContent](#addlinktocontent) | Creates a new custom document property which links to content. |
| [updateLinkedPropertyValue](#updatelinkedpropertyvalue) | Update custom document property value which links to content. |
| [updateLinkedRange](#updatelinkedrange) | Update custom document property value to linked range. |
| [contains](#contains) | Returns true if a property with the specified name exists in the collection. |
| [indexOf](#indexof) | Gets the index of a property by name. |
| [remove](#remove) | Removes a property with the specified name from the collection. |
| [removeAt](#removeat) | Removes a property at the specified index. |
| [clear](#clear) |  |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |

### CustomDocumentPropertyCollection.Count property {#count}

**Type:** Number

### CustomDocumentPropertyCollection.Item (java.lang.String) property {#itemjavalangstring}

Returns a DocumentProperty object by the name of the property. Returns null if a property with the specified name is not found.

**Type:** DocumentProperty

### CustomDocumentPropertyCollection.Item (int) property {#itemint}

Returns a DocumentProperty object by index.

**Type:** DocumentProperty

### add(name, value) (1 of 6) {#add}

Creates a new custom document property of the PropertyType.String data type.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property. |
| value | String | The value of the property. |

**Returns:** The newly created property object.

---

### add(name, value) (2 of 6) {#add-1}

Creates a new custom document property of the PropertyType.Number data type.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property. |
| value | Number | The value of the property. |

**Returns:** The newly created property object.

---

### add(name, value) (3 of 6) {#add-2}

Creates a new custom document property of the PropertyType.DateTime data type.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property. |
| value | DateTime | The value of the property. |

**Returns:** The newly created property object.

---

### add(name, value) (4 of 6) {#add-3}

Creates a new custom document property of the PropertyType.Boolean data type.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property. |
| value | boolean | The value of the property. |

**Returns:** The newly created property object.

---

### add(name, value) (5 of 6) {#add-4}

Creates a new custom document property of the PropertyType.Float data type.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property. |
| value | Number | The value of the property. |

**Returns:** The newly created property object.

---

### add(value) (6 of 6) {#add-5}

Reserved for internal use.

### addLinkToContent(name, source) {#addlinktocontent}

Creates a new custom document property which links to content.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property. |
| source | String | The source of the property |

**Returns:** The newly created property object.

### updateLinkedPropertyValue() {#updatelinkedpropertyvalue}

Update custom document property value which links to content.

### updateLinkedRange() {#updatelinkedrange}

Update custom document property value to linked range.

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
| index | Number | The zero based index. |

### clear() {#clear}

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.
