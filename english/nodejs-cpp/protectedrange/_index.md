---
title: ProtectedRange
second_title: Aspose.Cells for Node.js via C++ API Reference
description: A specified range to be allowed to edit when the sheet protection is ON.
type: docs
url: /nodejs-cpp/protectedrange/
---

## ProtectedRange class

A specified range to be allowed to edit when the sheet protection is ON.

```javascript
class ProtectedRange;
```


## Methods

| Method | Description |
| --- | --- |
| [getName()](#getName--)| Gets the Range title. This is used as a descriptor, not as a named range definition. |
| [setName(string)](#setName-string-)| Gets the Range title. This is used as a descriptor, not as a named range definition. |
| [getCellArea()](#getCellArea--)| Gets the [CellArea](/nodejs-cpp/cellarea/) object represents the cell area to be protected. |
| [isProtectedWithPassword()](#isProtectedWithPassword--)| Indicates whether the worksheets is protected with password. |
| [getPassword()](#getPassword--)| Represents the password to protect the range. |
| [setPassword(string)](#setPassword-string-)| Represents the password to protect the range. |
| [getSecurityDescriptor()](#getSecurityDescriptor--)| The security descriptor defines user accounts who may edit this range without providing a password to access the range. |
| [setSecurityDescriptor(string)](#setSecurityDescriptor-string-)| The security descriptor defines user accounts who may edit this range without providing a password to access the range. |
| [getAreas()](#getAreas--)| Gets all referred areas. |
| [addArea(number, number, number, number)](#addArea-number-number-number-number-)| Adds a referred area to this |


### getName() {#getName--}

Gets the Range title. This is used as a descriptor, not as a named range definition.

```javascript
getName() : string;
```


### setName(string) {#setName-string-}

Gets the Range title. This is used as a descriptor, not as a named range definition.

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getCellArea() {#getCellArea--}

Gets the [CellArea](/nodejs-cpp/cellarea/) object represents the cell area to be protected.

```javascript
getCellArea() : CellArea;
```


**Returns**

[CellArea](/nodejs-cpp/cellarea/)

### isProtectedWithPassword() {#isProtectedWithPassword--}

Indicates whether the worksheets is protected with password.

```javascript
isProtectedWithPassword() : boolean;
```


### getPassword() {#getPassword--}

Represents the password to protect the range.

```javascript
getPassword() : string;
```


### setPassword(string) {#setPassword-string-}

Represents the password to protect the range.

```javascript
setPassword(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getSecurityDescriptor() {#getSecurityDescriptor--}

The security descriptor defines user accounts who may edit this range without providing a password to access the range.

```javascript
getSecurityDescriptor() : string;
```


### setSecurityDescriptor(string) {#setSecurityDescriptor-string-}

The security descriptor defines user accounts who may edit this range without providing a password to access the range.

```javascript
setSecurityDescriptor(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getAreas() {#getAreas--}

Gets all referred areas.

```javascript
getAreas() : CellArea[];
```


**Returns**

Returns all referred areas.

### addArea(number, number, number, number) {#addArea-number-number-number-number-}

Adds a referred area to this

```javascript
addArea(startRow: number, startColumn: number, endRow: number, endColumn: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | The start row. |
| startColumn | number | The start column. |
| endRow | number | The end row. |
| endColumn | number | The end column. |


