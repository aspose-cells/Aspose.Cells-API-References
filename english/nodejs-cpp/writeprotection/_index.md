---
title: WriteProtection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Specifies write protection settings for a workbook.
type: docs
url: /nodejs-cpp/writeprotection/
---

## WriteProtection class

Specifies write protection settings for a workbook.

```javascript
class WriteProtection;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getAuthor()](#getAuthor--)| Gets and sets the author. |
| [setAuthor(string)](#setAuthor-string-)| Gets and sets the author. |
| [getRecommendReadOnly()](#getRecommendReadOnly--)| Indicates if the Read Only Recommended option is selected. |
| [setRecommendReadOnly(boolean)](#setRecommendReadOnly-boolean-)| Indicates if the Read Only Recommended option is selected. |
| [isWriteProtected()](#isWriteProtected--)| Indicates whether this workbook is write protected. |
| [getPassword()](#getPassword--)| Sets the protected password to modify the file. |
| [setPassword(string)](#setPassword-string-)| Sets the protected password to modify the file. |
| [validatePassword(string)](#validatePassword-string-)| Returns true if the specified password is the same as the write-protection password the file was protected with. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### getAuthor() {#getAuthor--}

Gets and sets the author.

```javascript
getAuthor() : string;
```


### setAuthor(string) {#setAuthor-string-}

Gets and sets the author.

```javascript
setAuthor(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getRecommendReadOnly() {#getRecommendReadOnly--}

Indicates if the Read Only Recommended option is selected.

```javascript
getRecommendReadOnly() : boolean;
```


### setRecommendReadOnly(boolean) {#setRecommendReadOnly-boolean-}

Indicates if the Read Only Recommended option is selected.

```javascript
setRecommendReadOnly(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isWriteProtected() {#isWriteProtected--}

Indicates whether this workbook is write protected.

```javascript
isWriteProtected() : boolean;
```


### getPassword() {#getPassword--}

Sets the protected password to modify the file.

```javascript
getPassword() : string;
```


### setPassword(string) {#setPassword-string-}

Sets the protected password to modify the file.

```javascript
setPassword(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### validatePassword(string) {#validatePassword-string-}

Returns true if the specified password is the same as the write-protection password the file was protected with.

```javascript
validatePassword(password: string) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | string | The specified password. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



