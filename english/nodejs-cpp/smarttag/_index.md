---
title: SmartTag
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a smart tag.
type: docs
url: /nodejs-cpp/smarttag/
---

## SmartTag class

Represents a smart tag.

```javascript
class SmartTag;
```


## Methods

| Method | Description |
| --- | --- |
| [getDeleted()](#getDeleted--)| Indicates whether the smart tag is deleted. |
| [setDeleted(boolean)](#setDeleted-boolean-)| Indicates whether the smart tag is deleted. |
| [getProperties()](#getProperties--)| Gets and set the properties of the smart tag. |
| [setProperties(SmartTagPropertyCollection)](#setProperties-smarttagpropertycollection-)| Gets and set the properties of the smart tag. |
| [getUri()](#getUri--)| Gets the namespace URI of the smart tag. |
| [getName()](#getName--)| Gets the name of the smart tag. |
| [setLink(string, string)](#setLink-string-string-)| Change the name and  the namespace URI of the smart tag. |


### getDeleted() {#getDeleted--}

Indicates whether the smart tag is deleted.

```javascript
getDeleted() : boolean;
```


### setDeleted(boolean) {#setDeleted-boolean-}

Indicates whether the smart tag is deleted.

```javascript
setDeleted(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getProperties() {#getProperties--}

Gets and set the properties of the smart tag.

```javascript
getProperties() : SmartTagPropertyCollection;
```


**Returns**

[SmartTagPropertyCollection](/nodejs-cpp/smarttagpropertycollection/)

### setProperties(SmartTagPropertyCollection) {#setProperties-smarttagpropertycollection-}

Gets and set the properties of the smart tag.

```javascript
setProperties(value: SmartTagPropertyCollection) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SmartTagPropertyCollection](/nodejs-cpp/smarttagpropertycollection/) | The value to set. |

### getUri() {#getUri--}

Gets the namespace URI of the smart tag.

```javascript
getUri() : string;
```


### getName() {#getName--}

Gets the name of the smart tag.

```javascript
getName() : string;
```


### setLink(string, string) {#setLink-string-string-}

Change the name and  the namespace URI of the smart tag.

```javascript
setLink(uri: string, name: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uri | string | The namespace URI of the smart tag. |
| name | string | The name of the smart tag. |


