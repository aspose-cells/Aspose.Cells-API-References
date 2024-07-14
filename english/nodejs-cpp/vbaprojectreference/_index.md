---
title: VbaProjectReference
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the reference of VBA project.
type: docs
url: /nodejs-cpp/vbaprojectreference/
---

## VbaProjectReference class

Represents the reference of VBA project.

```javascript
class VbaProjectReference;
```


## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| Gets the type of this reference. |
| [getName()](#getName--)| Gets and sets the name of the reference. |
| [setName(string)](#setName-string-)| Gets and sets the name of the reference. |
| [getLibid()](#getLibid--)| Gets and sets the Libid of the reference. |
| [setLibid(string)](#setLibid-string-)| Gets and sets the Libid of the reference. |
| [getTwiddledlibid()](#getTwiddledlibid--)| Gets and sets the twiddled Libid of the reference. |
| [setTwiddledlibid(string)](#setTwiddledlibid-string-)| Gets and sets the twiddled Libid of the reference. |
| [getExtendedLibid()](#getExtendedLibid--)| Gets and sets the extended Libid of the reference. |
| [setExtendedLibid(string)](#setExtendedLibid-string-)| Gets and sets the extended Libid of the reference. |
| [getRelativeLibid()](#getRelativeLibid--)| Gets and sets the referenced VBA project's identifier with an relative path. |
| [setRelativeLibid(string)](#setRelativeLibid-string-)| Gets and sets the referenced VBA project's identifier with an relative path. |
| [copy(VbaProjectReference)](#copy-vbaprojectreference-)|  |


### getType() {#getType--}

Gets the type of this reference.

```javascript
getType() : VbaProjectReferenceType;
```


**Returns**

[VbaProjectReferenceType](/nodejs-cpp/vbaprojectreferencetype/)

### getName() {#getName--}

Gets and sets the name of the reference.

```javascript
getName() : string;
```


### setName(string) {#setName-string-}

Gets and sets the name of the reference.

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getLibid() {#getLibid--}

Gets and sets the Libid of the reference.

```javascript
getLibid() : string;
```


### setLibid(string) {#setLibid-string-}

Gets and sets the Libid of the reference.

```javascript
setLibid(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getTwiddledlibid() {#getTwiddledlibid--}

Gets and sets the twiddled Libid of the reference.

```javascript
getTwiddledlibid() : string;
```


**Remarks**

Only for control reference.

### setTwiddledlibid(string) {#setTwiddledlibid-string-}

Gets and sets the twiddled Libid of the reference.

```javascript
setTwiddledlibid(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

Only for control reference.

### getExtendedLibid() {#getExtendedLibid--}

Gets and sets the extended Libid of the reference.

```javascript
getExtendedLibid() : string;
```


**Remarks**

Only for control reference.

### setExtendedLibid(string) {#setExtendedLibid-string-}

Gets and sets the extended Libid of the reference.

```javascript
setExtendedLibid(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

Only for control reference.

### getRelativeLibid() {#getRelativeLibid--}

Gets and sets the referenced VBA project's identifier with an relative path.

```javascript
getRelativeLibid() : string;
```


**Remarks**

Only for project reference.

### setRelativeLibid(string) {#setRelativeLibid-string-}

Gets and sets the referenced VBA project's identifier with an relative path.

```javascript
setRelativeLibid(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

Only for project reference.

### copy(VbaProjectReference) {#copy-vbaprojectreference-}



```javascript
copy(source: VbaProjectReference) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [VbaProjectReference](/nodejs-cpp/vbaprojectreference/) |  |


