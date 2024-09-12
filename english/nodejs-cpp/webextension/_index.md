---
title: WebExtension
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents an Office Addin instance.
type: docs
url: /nodejs-cpp/webextension/
---

## WebExtension class

Represents an Office Add-in instance.

```javascript
class WebExtension;
```


## Methods

| Method | Description |
| --- | --- |
| [getId()](#getId--)| Gets and sets the uniquely identifies the Office Add-in instance in the current document. |
| [setId(string)](#setId-string-)| Gets and sets the uniquely identifies the Office Add-in instance in the current document. |
| [isFrozen()](#isFrozen--)| Indicates whether the user can interact with the Office Add-in or not. |
| [setIsFrozen(boolean)](#setIsFrozen-boolean-)| Indicates whether the user can interact with the Office Add-in or not. |
| [getReference()](#getReference--)| Get the primary reference to an Office Add-in. |
| [getAlterReferences()](#getAlterReferences--)| Gets a list of alter references. |
| [getProperties()](#getProperties--)| Gets all properties of web extension. |
| [getBindings()](#getBindings--)| Gets all bindings relationship between an Office Add-in and the data in the document. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getId() {#getId--}

Gets and sets the uniquely identifies the Office Add-in instance in the current document.

```javascript
getId() : string;
```


### setId(string) {#setId-string-}

Gets and sets the uniquely identifies the Office Add-in instance in the current document.

```javascript
setId(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isFrozen() {#isFrozen--}

Indicates whether the user can interact with the Office Add-in or not.

```javascript
isFrozen() : boolean;
```


### setIsFrozen(boolean) {#setIsFrozen-boolean-}

Indicates whether the user can interact with the Office Add-in or not.

```javascript
setIsFrozen(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getReference() {#getReference--}

Get the primary reference to an Office Add-in.

```javascript
getReference() : WebExtensionReference;
```


**Returns**

[WebExtensionReference](../webextensionreference/)

### getAlterReferences() {#getAlterReferences--}

Gets a list of alter references.

```javascript
getAlterReferences() : WebExtensionReferenceCollection;
```


**Returns**

[WebExtensionReferenceCollection](../webextensionreferencecollection/)

### getProperties() {#getProperties--}

Gets all properties of web extension.

```javascript
getProperties() : WebExtensionPropertyCollection;
```


**Returns**

[WebExtensionPropertyCollection](../webextensionpropertycollection/)

### getBindings() {#getBindings--}

Gets all bindings relationship between an Office Add-in and the data in the document.

```javascript
getBindings() : WebExtensionBindingCollection;
```


**Returns**

[WebExtensionBindingCollection](../webextensionbindingcollection/)

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



