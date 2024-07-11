---
title: PageStartSavingArgs
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Info for a page starts saving process.
type: docs
url: /nodejs-cpp/pagestartsavingargs/
---

## PageStartSavingArgs class

Info for a page starts saving process.

```javascript
class PageStartSavingArgs extends PageSavingArgs;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(PageSavingArgs)](#constructor-pagesavingargs-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [isToOutput()](#isToOutput--)| Gets or sets a value indicating whether the page should be output. The default value is true. |
| [setIsToOutput(boolean)](#setIsToOutput-boolean-)| Gets or sets a value indicating whether the page should be output. The default value is true. |
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

### isToOutput() {#isToOutput--}

Gets or sets a value indicating whether the page should be output. The default value is true.

```javascript
isToOutput() : boolean;
```


### setIsToOutput(boolean) {#setIsToOutput-boolean-}

Gets or sets a value indicating whether the page should be output. The default value is true.

```javascript
setIsToOutput(value: boolean) : void;
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



