---
title: FolderFontSource
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the folder that contains TrueType font files.
type: docs
url: /nodejs-cpp/folderfontsource/
---

## FolderFontSource class

Represents the folder that contains TrueType font files.

```javascript
class FolderFontSource extends FontSourceBase;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(FontSourceBase)](#constructor-fontsourcebase-)| Constructs from a parent object convertible to this. |
| [constructor(string, boolean)](#constructor-string-boolean-)| Ctor. |

## Methods

| Method | Description |
| --- | --- |
| [getFolderPath()](#getFolderPath--)| Path to fonts folder. |
| [getScanSubFolders()](#getScanSubFolders--)| Determines whether or not to scan the subfolders. |
| [getType()](#getType--)| Returns the type of the font source. |


### constructor(FontSourceBase) {#constructor-fontsourcebase-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: FontSourceBase);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | FontSourceBase | The parent object. |

### constructor(string, boolean) {#constructor-string-boolean-}

Ctor.

```javascript
constructor(folderPath: string, scanSubfolders: boolean);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| folderPath | string | path to fonts folder |
| scanSubfolders | boolean | Determines whether or not to scan subfolders. |

### getFolderPath() {#getFolderPath--}

Path to fonts folder.

```javascript
getFolderPath() : string;
```


### getScanSubFolders() {#getScanSubFolders--}

Determines whether or not to scan the subfolders.

```javascript
getScanSubFolders() : boolean;
```


### getType() {#getType--}

Returns the type of the font source.

```javascript
getType() : FontSourceType;
```


**Returns**

[FontSourceType](../fontsourcetype/)


