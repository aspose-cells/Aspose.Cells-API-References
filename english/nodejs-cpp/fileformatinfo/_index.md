---
title: FileFormatInfo
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Contains data returned by FileFormatUtil..fileformatutil file format detection methods.
type: docs
url: /nodejs-cpp/fileformatinfo/
---

## FileFormatInfo class

Contains data returned by [FileFormatUtil](../fileformatutil/) file format detection methods.

```javascript
class FileFormatInfo;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [isProtectedByRMS()](#isProtectedByRMS--)| Gets whether the file is protected by Microsoft Rights Management Server. |
| [isEncrypted()](#isEncrypted--)| Returns true if the document is encrypted and requires a password to open. |
| [getFileFormatType()](#getFileFormatType--)| Gets the detected file format. |
| [getLoadFormat()](#getLoadFormat--)| Gets the detected load format. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### isProtectedByRMS() {#isProtectedByRMS--}

Gets whether the file is protected by Microsoft Rights Management Server.

```javascript
isProtectedByRMS() : boolean;
```


### isEncrypted() {#isEncrypted--}

Returns true if the document is encrypted and requires a password to open.

```javascript
isEncrypted() : boolean;
```


### getFileFormatType() {#getFileFormatType--}

Gets the detected file format.

```javascript
getFileFormatType() : FileFormatType;
```


**Returns**

[FileFormatType](../fileformattype/)

### getLoadFormat() {#getLoadFormat--}

Gets the detected load format.

```javascript
getLoadFormat() : LoadFormat;
```


**Returns**

[LoadFormat](../loadformat/)


