﻿---
title: ExternalLinkCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents external links collection in a workbook.
type: docs
url: /nodejs-cpp/externallinkcollection/
---

## ExternalLinkCollection class

Represents external links collection in a workbook.

```javascript
class ExternalLinkCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [ExternalLink](../externallink/) element at the specified index. |
| [getCount()](#getCount--)| Gets the number of elements actually contained in the collection. |
| [add(string, string[])](#add-string-stringarray-)| Adds an external link. |
| [add(DirectoryType, string, string[])](#add-directorytype-string-stringarray-)| Add an external link . |
| [clear()](#clear--)| Removes all external links. |
| [clear(boolean)](#clear-boolean-)| Removes all external links. |
| [removeAt(number)](#removeAt-number-)| Removes the specified external link from the workbook. |
| [removeAt(number, boolean)](#removeAt-number-boolean-)| Removes the specified external link from the workbook. |
| [getEnumerator()](#getEnumerator--)| Get an enumerator that iterates through this collection. |


### get(number) {#get-number-}

Gets the [ExternalLink](../externallink/) element at the specified index.

```javascript
get(index: number) : ExternalLink;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |

**Returns**

The element at the specified index.

### getCount() {#getCount--}

Gets the number of elements actually contained in the collection.

```javascript
getCount() : number;
```


### add(string, string[]) {#add-string-stringarray-}

Adds an external link.

```javascript
add(fileName: string, sheetNames: string[]) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | string | The external file name. |
| sheetNames | string[] | All sheet names of the external file. |

**Returns**

The position of the external name in this list.

### add(DirectoryType, string, string[]) {#add-directorytype-string-stringarray-}

Add an external link .

```javascript
add(directoryType: DirectoryType, fileName: string, sheetNames: string[]) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directoryType | [DirectoryType](../directorytype/) | The directory type of the file name. |
| fileName | string | the file name. |
| sheetNames | string[] | All sheet names of the external file. |

**Returns**

The position of the external name in this list.

### clear() {#clear--}

Removes all external links.

```javascript
clear() : void;
```


**Remarks**

When removing external links, all formulas that reference to them will be removed too because the references become invalid.

### clear(boolean) {#clear-boolean-}

Removes all external links.

```javascript
clear(updateReferencesAsLocal: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| updateReferencesAsLocal | boolean | Whether update all references of external links in formulas to references of current workbook itself. |

**Remarks**

If references are required to be updated, those references of external links in formulas will be changed to current workbook when it is possible. For example, one cell's original formula is "='externalsource.xlam'!customfunction()", after removing external links, the formula will become "=customfunction()"; When the original formula is "='[externalsource.xlam]Sheet1'!$A$1", according to whether there is one sheet with name "Sheet1" in current workbook: if true, the formula will become "=Sheet1!$A$1"; if false, the formula will become "=#REF!$A$1".<br></br> If references are not required to be updated, all formulas with references to external links will be removed too because those references become invalid.

### removeAt(number) {#removeAt-number-}

Removes the specified external link from the workbook.

```javascript
removeAt(index: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | the index of the external link to be removed. |

**Remarks**

When removing the external link, all formulas that reference to it will be removed too because the references become invalid.

### removeAt(number, boolean) {#removeAt-number-boolean-}

Removes the specified external link from the workbook.

```javascript
removeAt(index: number, updateReferencesAsLocal: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | the index of the external link to be removed. |
| updateReferencesAsLocal | boolean | Whether update all references of given external link to reference of current workbook itself.         /// Check [Clear(bool)](../clear(bool)/) to get more details about this parameter. |

### getEnumerator() {#getEnumerator--}

Get an enumerator that iterates through this collection.

```javascript
getEnumerator() : ExternalLinkEnumerator;
```


**Returns**

[ExternalLinkEnumerator](../externallinkenumerator/)


