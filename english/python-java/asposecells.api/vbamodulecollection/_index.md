---
title: "VbaModuleCollection Class"
linktitle: "VbaModuleCollection"
articleTitle: "VbaModuleCollection"
second_title: "Aspose.Cells for Python via Java"
description: "Represents the list of VbaModule"
type: docs
weight: 7280
url: /python-java/asposecells.api/vbamodulecollection/
---

## VbaModuleCollection class

Represents the list of VbaModule

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | int |  |
| [Item (int)](#itemint) | VbaModule | Gets VbaModule in the list by the index. |
| [Item (java.lang.String)](#itemjavalangstring) | VbaModule | Gets VbaModule in the list by the name. |

## Methods

| Name | Description |
| --- | --- |
| [addDesignerStorage](#adddesignerstorage) |  |
| [getDesignerStorage](#getdesignerstorage) | Represents the data of Designer.

We do not support to parse them. Just only for copying. |
| [add](#add) | Adds module for a worksheet. |
| [addUserForm](#adduserform) | Inser user form into VBA Project. |
| [remove](#remove) | Removes module for a worksheet. |
| [clear](#clear) |  |
| [removeAt](#removeat) |  |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### VbaModuleCollection.Count property {#count}

**Type:** int

### VbaModuleCollection.Item (int) property {#itemint}

Gets VbaModule in the list by the index.

**Type:** VbaModule

### VbaModuleCollection.Item (java.lang.String) property {#itemjavalangstring}

Gets VbaModule in the list by the name.

**Type:** VbaModule

### addDesignerStorage(name, data) {#adddesignerstorage}

| Parameter | Type | Description |
| --- | --- | --- |
| name | String |  |
| data | byte[] |  |

### getDesignerStorage(name) {#getdesignerstorage}

Represents the data of Designer.

We do not support to parse them. Just only for copying.

### add(sheet) (1 of 3) {#add}

Adds module for a worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| sheet | Worksheet | The worksheet |

---

### add(type, name) (2 of 3) {#add-1}

Adds module.

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A VbaModuleType value. The type of module. |
| name | String | The name of module. |

---

### add(value) (3 of 3) {#add-2}

Reserved for internal use.

### addUserForm(name, codes, designerStorage) {#adduserform}

Inser user form into VBA Project.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of user form |
| codes | String | The codes for the user form |
| designerStorage | byte[] | the designer setting about the user form |

### remove(sheet) (1 of 2) {#remove}

Removes module for a worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| sheet | Worksheet | The worksheet |

---

### remove(name) (2 of 2) {#remove-1}

Remove the module by the name

| Parameter | Type | Description |
| --- | --- | --- |
| name | String |  |

### clear() {#clear}

### removeAt(index) {#removeat}

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.
