---
title: "ExternalLinkCollection"
linktitle: "ExternalLinkCollection"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents external links collection in a workbook."
type: docs
weight: 1400
url: /nodejs/aspose.cells/externallinkcollection/
---

## ExternalLinkCollection class

Represents external links collection in a workbook.

## Methods

| Name | Description |
| --- | --- |
| [add(fileName, sheetNames)](#add) | Adds an external link. |
| [add(directoryType, fileName, sheetNames)](#add-1) | Add an external link . |
| [clear()](#clear) | Removes all external links. When removing external links, all formulas that reference to them will be removed too becaus |
| [clear(updateReferencesAsLocal)](#clear-1) | Removes all external links. If references are required to be updated, those references of external links in formulas wil |
| [get(index)](#get) | Gets the ExternalLink element at the specified index. |
| [getCount()](#getcount) | Gets the number of elements actually contained in the collection. |
| [iterator()](#iterator) | Get an enumerator that iterates through this collection. |
| [removeAt(index)](#removeat) | Removes the specified external link from the workbook. When removing the external link, all formulas that reference to i |
| [removeAt(index, updateReferencesAsLocal)](#removeat-1) | Removes the specified external link from the workbook. |

### add(fileName, sheetNames) {#add}

Adds an external link.

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The external file name. |
| sheetNames | Array of String | All sheet names of the external file. |

**Returns:** Number — `Number` The position of the external name in this list.

### add(directoryType, fileName, sheetNames) {#add-1}

Add an external link .

| Parameter | Type | Description |
| --- | --- | --- |
| directoryType | Number | DirectoryType |
| fileName | String | the file name. |
| sheetNames | Array of String | All sheet names of the external file. |

**Returns:** Number — `Number` The position of the external name in this list.

### clear() {#clear}

Removes all external links. When removing external links, all formulas that reference to them will be removed too because the references become invalid.

### clear(updateReferencesAsLocal) {#clear-1}

Removes all external links. If references are required to be updated, those references of external links in formulas will be changed to current workbook when it is possible. For example, one cell's original formula is "='externalsource.xlam'!customfunction()", after removing external links, the formula will become "=customfunction()"; When the original formula is "='[externalsource.xlam]Sheet1'!$A$1", according to whether there is one sheet with name "Sheet1" in current workbook: if true, the formula will become "=Sheet1!$A$1"; if false, the formula will become "=#REF!$A$1". If references are not required to be updated, all formulas with references to external links will be removed too because those references become invalid.

| Parameter | Type | Description |
| --- | --- | --- |
| updateReferencesAsLocal | boolean | Whether update all references of external links in formulas to references of current workbook itself. |

### get(index) {#get}

Gets the ExternalLink element at the specified index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The zero based index of the element. |

**Returns:** ExternalLink — `ExternalLink` The element at the specified index.

### getCount() {#getcount}

Gets the number of elements actually contained in the collection.

### iterator() {#iterator}

Get an enumerator that iterates through this collection.

**Returns:** Iterator — `Iterator`

### removeAt(index) {#removeat}

Removes the specified external link from the workbook. When removing the external link, all formulas that reference to it will be removed too because the references become invalid.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | the index of the external link to be removed. |

### removeAt(index, updateReferencesAsLocal) {#removeat-1}

Removes the specified external link from the workbook.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | the index of the external link to be removed. |
| updateReferencesAsLocal | boolean | Whether update all references of given external link to reference of current workbook itself. Check |
