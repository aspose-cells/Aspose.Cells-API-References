---
title: PageEndSavingArgs
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Info for a page ends saving process.
type: docs
url: /nodejs-cpp/pageendsavingargs/
---

## PageEndSavingArgs class

Info for a page ends saving process.

```javascript
class PageEndSavingArgs extends PageSavingArgs;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(PageSavingArgs)](#constructor-pagesavingargs-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getHasMorePages()](#getHasMorePages--)| Gets or sets a value indicating whether having more pages to be output. The default value is true. |
| [setHasMorePages(boolean)](#setHasMorePages-boolean-)| Gets or sets a value indicating whether having more pages to be output. The default value is true. |
| [getPageIndex()](#getPageIndex--)| Current page index, zero based. |
| [getPageCount()](#getPageCount--)| Total page count. |


### constructor(PageSavingArgs) {#constructor-pagesavingargs-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: PageSavingArgs);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | PageSavingArgs | The parent object. |

### getHasMorePages() {#getHasMorePages--}

Gets or sets a value indicating whether having more pages to be output. The default value is true.

```javascript
getHasMorePages() : boolean;
```


### setHasMorePages(boolean) {#setHasMorePages-boolean-}

Gets or sets a value indicating whether having more pages to be output. The default value is true.

```javascript
setHasMorePages(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getPageIndex() {#getPageIndex--}

Current page index, zero based.

```javascript
getPageIndex() : number;
```


### getPageCount() {#getPageCount--}

Total page count.

```javascript
getPageCount() : number;
```



