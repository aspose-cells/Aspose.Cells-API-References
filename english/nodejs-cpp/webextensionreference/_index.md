---
title: WebExtensionReference
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents identify the provider location and version of the extension.
type: docs
url: /nodejs-cpp/webextensionreference/
---

## WebExtensionReference class

Represents identify the provider location and version of the extension.

```javascript
class WebExtensionReference;
```


## Methods

| Method | Description |
| --- | --- |
| [getId()](#getId--)| Gets and sets the identifier associated with the Office Add-in within a catalog provider. The identifier MUST be unique within a catalog provider. |
| [setId(string)](#setId-string-)| Gets and sets the identifier associated with the Office Add-in within a catalog provider. The identifier MUST be unique within a catalog provider. |
| [getVersion()](#getVersion--)| Gets and sets the version. |
| [setVersion(string)](#setVersion-string-)| Gets and sets the version. |
| [getStoreName()](#getStoreName--)| Gets and sets the instance of the marketplace where the Office Add-in is stored. . |
| [setStoreName(string)](#setStoreName-string-)| Gets and sets the instance of the marketplace where the Office Add-in is stored. . |
| [getStoreType()](#getStoreType--)| Gets and sets the type of marketplace that the store attribute identifies. |
| [setStoreType(WebExtensionStoreType)](#setStoreType-webextensionstoretype-)| Gets and sets the type of marketplace that the store attribute identifies. |


### getId() {#getId--}

Gets and sets the identifier associated with the Office Add-in within a catalog provider. The identifier MUST be unique within a catalog provider.

```javascript
getId() : string;
```


### setId(string) {#setId-string-}

Gets and sets the identifier associated with the Office Add-in within a catalog provider. The identifier MUST be unique within a catalog provider.

```javascript
setId(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getVersion() {#getVersion--}

Gets and sets the version.

```javascript
getVersion() : string;
```


### setVersion(string) {#setVersion-string-}

Gets and sets the version.

```javascript
setVersion(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getStoreName() {#getStoreName--}

Gets and sets the instance of the marketplace where the Office Add-in is stored. .

```javascript
getStoreName() : string;
```


### setStoreName(string) {#setStoreName-string-}

Gets and sets the instance of the marketplace where the Office Add-in is stored. .

```javascript
setStoreName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getStoreType() {#getStoreType--}

Gets and sets the type of marketplace that the store attribute identifies.

```javascript
getStoreType() : WebExtensionStoreType;
```


**Returns**

[WebExtensionStoreType](../webextensionstoretype/)

### setStoreType(WebExtensionStoreType) {#setStoreType-webextensionstoretype-}

Gets and sets the type of marketplace that the store attribute identifies.

```javascript
setStoreType(value: WebExtensionStoreType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [WebExtensionStoreType](../webextensionstoretype/) | The value to set. |


