---
title: "ExternalLinkCollection Class"
linktitle: "ExternalLinkCollection"
articleTitle: "ExternalLinkCollection"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents external links collection in a workbook."
type: docs
weight: 2210
url: /php/aspose.cells/externallinkcollection/
---

## ExternalLinkCollection class

Represents external links collection in a workbook.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Count](#count) | Number | Gets the number of elements actually contained in the collection. |
| [Item (int)](#itemint) | ExternalLink | Gets the ExternalLink element at the specified index. |

## Methods

| Name | Description |
| --- | --- |
| [add](#add) | Adds an external link. |
| [clear](#clear) | Removes all external links.

When removing external links, all formulas that reference to them will be removed too becau |
| [removeAt](#removeat) | Removes the specified external link from the workbook.

When removing the external link, all formulas that reference to  |
| [iterator](#iterator) | Get an enumerator that iterates through this collection. |

### ExternalLinkCollection.Count property {#count}

Gets the number of elements actually contained in the collection.

**Type:** Number

### ExternalLinkCollection.Item (int) property {#itemint}

Gets the ExternalLink element at the specified index.

**Type:** ExternalLink

### add(fileName, sheetNames) (1 of 2) {#add}

Adds an external link.

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The external file name. |
| sheetNames | String[] | All sheet names of the external file. |

**Returns:** The position of the external name in this list.

---

### add(directoryType, fileName, sheetNames) (2 of 2) {#add-1}

Add an external link .

| Parameter | Type | Description |
| --- | --- | --- |
| directoryType | Number | A DirectoryType value. The directory type of the file name. |
| fileName | String | the file name. |
| sheetNames | String[] | All sheet names of the external file. |

**Returns:** The position of the external name in this list.

### clear() (1 of 2) {#clear}

Removes all external links.

When removing external links, all formulas that reference to them will be removed too because the references become invalid.

---

### clear(updateReferencesAsLocal) (2 of 2) {#clear-1}

Removes all external links.

If references are required to be updated, those references of external links in formulas will be changed to current workbook when it is possible. For example, one cell's original formula is "='externalsource.xlam'!customfunction()", after removing external links, the formula will become "=customfunction()"; When the original formula is "='[externalsource.xlam]Sheet1'!$A$1", according to whether there is one sheet with name "Sheet1" in current workbook: if true, the formula will become "=Sheet1!$A$1"; if false, the formula will become "=#REF!$A$1". If references are not required to be updated, all formulas with references to external links will be removed too because those references become invalid.

| Parameter | Type | Description |
| --- | --- | --- |
| updateReferencesAsLocal | boolean | Whether update all references of external links in formulas to references of current workbook itself. |

### removeAt(index) (1 of 2) {#removeat}

Removes the specified external link from the workbook.

When removing the external link, all formulas that reference to it will be removed too because the references become invalid.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | the index of the external link to be removed. |

---

### removeAt(index, updateReferencesAsLocal) (2 of 2) {#removeat-1}

Removes the specified external link from the workbook.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | the index of the external link to be removed. |
| updateReferencesAsLocal | boolean | Whether update all references of given external link to reference of current workbook itself. Check clear(boolean) to get more details about this parameter. |

### iterator() {#iterator}

Get an enumerator that iterates through this collection.
