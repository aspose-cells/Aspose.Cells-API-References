---
title: "VbaModuleCollection"
linktitle: "VbaModuleCollection"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents the list of VbaModule"
type: docs
weight: 4470
url: /nodejs/aspose.cells/vbamodulecollection/
---

## VbaModuleCollection class

Represents the list of VbaModule

## Methods

| Name | Description |
| --- | --- |
| [add(sheet)](#add) | Adds module for a worksheet. |
| [add(type, name)](#add-1) | Adds module. |
| [add()](#add-2) | Reserved for internal use. |
| [addDesignerStorage(name, data)](#adddesignerstorage) |  |
| [addUserForm(name, codes, designerStorage)](#adduserform) | Inser user form into VBA Project. |
| [clear()](#clear) |  |
| [contains()](#contains) | Reserved for internal use. |
| [get(index)](#get) | Gets VbaModule in the list by the index. |
| [get(name)](#get-1) | Gets VbaModule in the list by the name. |
| [get()](#get-2) | Reserved for internal use. |
| [getCount()](#getcount) |  |
| [getDesignerStorage()](#getdesignerstorage) | Represents the data of Designer. We do not support to parse them. Just only for copying. |
| [indexOf()](#indexof) | Reserved for internal use. |
| [iterator()](#iterator) |  |
| [remove(sheet)](#remove) | Removes module for a worksheet. |
| [remove(name)](#remove-1) | Remove the module by the name |
| [removeAt()](#removeat) |  |

### add(sheet) {#add}

Adds module for a worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| sheet | Worksheet | The worksheet |

**Returns:** Number — `Number`

### add(type, name) {#add-1}

Adds module.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | VbaModuleType |
| name | String | The name of module. |

**Returns:** Number — `Number`

### add() {#add-2}

Reserved for internal use.

### addDesignerStorage(name, data) {#adddesignerstorage}

| Parameter | Type | Description |
| --- | --- | --- |
| name | String |  |
| data | Array of byte |  |

### addUserForm(name, codes, designerStorage) {#adduserform}

Inser user form into VBA Project.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of user form |
| codes | String | The codes for the user form |
| designerStorage | Array of byte | the designer setting about the user form |

**Returns:** Number — `Number`

### clear() {#clear}

### contains() {#contains}

Reserved for internal use.

### get(index) {#get}

Gets VbaModule in the list by the index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The index. |

**Returns:** VbaModule — `VbaModule`

### get(name) {#get-1}

Gets VbaModule in the list by the name.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of module. |

**Returns:** VbaModule — `VbaModule`

### get() {#get-2}

Reserved for internal use.

### getCount() {#getcount}

### getDesignerStorage() {#getdesignerstorage}

Represents the data of Designer. We do not support to parse them. Just only for copying.

### indexOf() {#indexof}

Reserved for internal use.

### iterator() {#iterator}

### remove(sheet) {#remove}

Removes module for a worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| sheet | Worksheet | The worksheet |

**Returns:** void — `void`

### remove(name) {#remove-1}

Remove the module by the name

| Parameter | Type | Description |
| --- | --- | --- |
| name | String |  |

### removeAt() {#removeat}
