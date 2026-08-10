---
title: "CustomDocumentPropertyCollection"
linktitle: "CustomDocumentPropertyCollection"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "A collection of custom document properties."
type: docs
weight: 880
url: /nodejs/aspose.cells/customdocumentpropertycollection/
---

## CustomDocumentPropertyCollection class

A collection of custom document properties. Each DocumentProperty object represents a custom property of a container document.

## Methods

| Name | Description |
| --- | --- |
| [add(name, value)](#add) | Creates a new custom document property of the PropertyType.String data type. |
| [add(name, value)](#add-1) | Creates a new custom document property of the PropertyType.Number data type. |
| [add(name, value)](#add-2) | Creates a new custom document property of the PropertyType.DateTime data type. |
| [add(name, value)](#add-3) | Creates a new custom document property of the PropertyType.Boolean data type. |
| [add(name, value)](#add-4) | Creates a new custom document property of the PropertyType.Float data type. |
| [add()](#add-5) | Reserved for internal use. |
| [addLinkToContent(name, source)](#addlinktocontent) | Creates a new custom document property which links to content. |
| [clear()](#clear) |  |
| [contains(name)](#contains) | Returns true if a property with the specified name exists in the collection. |
| [contains()](#contains-1) | Reserved for internal use. |
| [get(name)](#get) | Returns a DocumentProperty object by the name of the property. Returns null if a property with the specified name is not |
| [get(index)](#get-1) | Returns a DocumentProperty object by index. |
| [get()](#get-2) | Reserved for internal use. |
| [getCount()](#getcount) |  |
| [indexOf(name)](#indexof) | Gets the index of a property by name. |
| [indexOf()](#indexof-1) | Reserved for internal use. |
| [iterator()](#iterator) |  |
| [remove(name)](#remove) | Removes a property with the specified name from the collection. |
| [removeAt(index)](#removeat) | Removes a property at the specified index. |
| [updateLinkedPropertyValue()](#updatelinkedpropertyvalue) | Update custom document property value which links to content. |
| [updateLinkedRange()](#updatelinkedrange) | Update custom document property value to linked range. |

### add(name, value) {#add}

Creates a new custom document property of the PropertyType.String data type.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property. |
| value | String | The value of the property. |

**Returns:** DocumentProperty — `DocumentProperty` The newly created property object.

### add(name, value) {#add-1}

Creates a new custom document property of the PropertyType.Number data type.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property. |
| value | Number | The value of the property. |

**Returns:** DocumentProperty — `DocumentProperty` The newly created property object.

### add(name, value) {#add-2}

Creates a new custom document property of the PropertyType.DateTime data type.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property. |
| value | DateTime | The value of the property. |

**Returns:** DocumentProperty — `DocumentProperty` The newly created property object.

### add(name, value) {#add-3}

Creates a new custom document property of the PropertyType.Boolean data type.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property. |
| value | boolean | The value of the property. |

**Returns:** DocumentProperty — `DocumentProperty` The newly created property object.

### add(name, value) {#add-4}

Creates a new custom document property of the PropertyType.Float data type.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property. |
| value | Number | The value of the property. |

**Returns:** DocumentProperty — `DocumentProperty` The newly created property object.

### add() {#add-5}

Reserved for internal use.

### addLinkToContent(name, source) {#addlinktocontent}

Creates a new custom document property which links to content.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property. |
| source | String | The source of the property |

**Returns:** DocumentProperty — `DocumentProperty` The newly created property object.

### clear() {#clear}

### contains(name) {#contains}

Returns true if a property with the specified name exists in the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The case-insensitive name of the property. |

**Returns:** boolean — `boolean` True if the property exists in the collection; false otherwise.

### contains() {#contains-1}

Reserved for internal use.

### get(name) {#get}

Returns a DocumentProperty object by the name of the property. Returns null if a property with the specified name is not found.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The case-insensitive name of the property to retrieve. |

### get(index) {#get-1}

Returns a DocumentProperty object by index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | Zero-based index of the |

### get() {#get-2}

Reserved for internal use.

### getCount() {#getcount}

### indexOf(name) {#indexof}

Gets the index of a property by name.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The case-insensitive name of the property. |

**Returns:** Number — `Number` The zero based index. Negative value if not found.

### indexOf() {#indexof-1}

Reserved for internal use.

### iterator() {#iterator}

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

### updateLinkedPropertyValue() {#updatelinkedpropertyvalue}

Update custom document property value which links to content.

### updateLinkedRange() {#updatelinkedrange}

Update custom document property value to linked range.
