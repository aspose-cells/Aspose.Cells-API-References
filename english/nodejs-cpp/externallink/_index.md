---
title: ExternalLink
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents an external link in a workbook.
type: docs
url: /nodejs-cpp/externallink/
---

## ExternalLink class

Represents an external link in a workbook.

```javascript
class ExternalLink;
```


## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| Gets the type of external link. |
| [getPathType()](#getPathType--)| Get the path type of this external link |
| [getOriginalDataSource()](#getOriginalDataSource--)| Represents stored data source of the external link. |
| [setOriginalDataSource(string)](#setOriginalDataSource-string-)| Represents stored data source of the external link. |
| [getDataSource()](#getDataSource--)| Represents data source of the external link. |
| [setDataSource(string)](#setDataSource-string-)| Represents data source of the external link. |
| [isReferred()](#isReferred--)| Indicates whether this external link is referenced by others. |
| [isVisible()](#isVisible--)| Indicates whether this external link is visible in MS Excel. |
| [addExternalName(string, string)](#addExternalName-string-string-)| Adds an external name. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getType() {#getType--}

Gets the type of external link.

```javascript
getType() : ExternalLinkType;
```


**Returns**

[ExternalLinkType](../externallinktype/)

### getPathType() {#getPathType--}

Get the path type of this external link

```javascript
getPathType() : string;
```


### getOriginalDataSource() {#getOriginalDataSource--}

Represents stored data source of the external link.

```javascript
getOriginalDataSource() : string;
```


### setOriginalDataSource(string) {#setOriginalDataSource-string-}

Represents stored data source of the external link.

```javascript
setOriginalDataSource(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getDataSource() {#getDataSource--}

Represents data source of the external link.

```javascript
getDataSource() : string;
```


### setDataSource(string) {#setDataSource-string-}

Represents data source of the external link.

```javascript
setDataSource(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isReferred() {#isReferred--}

Indicates whether this external link is referenced by others.

```javascript
isReferred() : boolean;
```


### isVisible() {#isVisible--}

Indicates whether this external link is visible in MS Excel.

```javascript
isVisible() : boolean;
```


### addExternalName(string, string) {#addExternalName-string-string-}

Adds an external name.

```javascript
addExternalName(text: string, referTo: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | string | The text of the external name.         /// If the external name belongs to a worksheet, the text should be as Sheet1!Text. |
| referTo | string | The referTo of the external name. It must be a cell or the range. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



