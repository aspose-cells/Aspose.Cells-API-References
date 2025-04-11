---
title: VbaProject
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the VBA project.
type: docs
url: /nodejs-cpp/vbaproject/
---

## VbaProject class

Represents the VBA project.

```javascript
class VbaProject;
```


## Methods

| Method | Description |
| --- | --- |
| [isValidSigned()](#isValidSigned--)| Indicates whether the signature of VBA project is valid or not. |
| [getCertRawData()](#getCertRawData--)| Gets certificate raw data if this VBA project is signed. |
| [getEncoding()](#getEncoding--)| Gets and sets the encoding of VBA project. |
| [setEncoding(EncodingType)](#setEncoding-encodingtype-)| Gets and sets the encoding of VBA project. |
| [getName()](#getName--)| Gets and sets the name of the VBA project. |
| [setName(string)](#setName-string-)| Gets and sets the name of the VBA project. |
| [isSigned()](#isSigned--)| Indicates whether VBAcode is signed or not. |
| [isProtected()](#isProtected--)| Indicates whether this VBA project is protected. |
| [getIslockedForViewing()](#getIslockedForViewing--)| Indicates whether this VBA project is locked for viewing. |
| [getModules()](#getModules--)| Gets all [VbaModule](../vbamodule/) objects. |
| [getReferences()](#getReferences--)| Gets all references of VBA project. |
| [sign(DigitalSignature)](#sign-digitalsignature-)| Sign this VBA project by a DigitalSignature |
| [protect(boolean, string)](#protect-boolean-string-)| Protects or unprotects this VBA project. |
| [copy(VbaProject)](#copy-vbaproject-)| Copy VBA project from other file. |
| [validatePassword(string)](#validatePassword-string-)| Validates protection password. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### isValidSigned() {#isValidSigned--}

Indicates whether the signature of VBA project is valid or not.

```javascript
isValidSigned() : boolean;
```


### getCertRawData() {#getCertRawData--}

Gets certificate raw data if this VBA project is signed.

```javascript
getCertRawData() : Uint8Array;
```


### getEncoding() {#getEncoding--}

Gets and sets the encoding of VBA project.

```javascript
getEncoding() : EncodingType;
```


**Returns**

[EncodingType](../encodingtype/)

### setEncoding(EncodingType) {#setEncoding-encodingtype-}

Gets and sets the encoding of VBA project.

```javascript
setEncoding(value: EncodingType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [EncodingType](../encodingtype/) | The value to set. |

### getName() {#getName--}

Gets and sets the name of the VBA project.

```javascript
getName() : string;
```


### setName(string) {#setName-string-}

Gets and sets the name of the VBA project.

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isSigned() {#isSigned--}

Indicates whether VBAcode is signed or not.

```javascript
isSigned() : boolean;
```


### isProtected() {#isProtected--}

Indicates whether this VBA project is protected.

```javascript
isProtected() : boolean;
```


### getIslockedForViewing() {#getIslockedForViewing--}

Indicates whether this VBA project is locked for viewing.

```javascript
getIslockedForViewing() : boolean;
```


### getModules() {#getModules--}

Gets all [VbaModule](../vbamodule/) objects.

```javascript
getModules() : VbaModuleCollection;
```


**Returns**

[VbaModuleCollection](../vbamodulecollection/)

### getReferences() {#getReferences--}

Gets all references of VBA project.

```javascript
getReferences() : VbaProjectReferenceCollection;
```


**Returns**

[VbaProjectReferenceCollection](../vbaprojectreferencecollection/)

### sign(DigitalSignature) {#sign-digitalsignature-}

Sign this VBA project by a DigitalSignature

```javascript
sign(digitalSignature: DigitalSignature) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| digitalSignature | [DigitalSignature](../digitalsignature/) | DigitalSignature |

### protect(boolean, string) {#protect-boolean-string-}

Protects or unprotects this VBA project.

```javascript
protect(islockedForViewing: boolean, password: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| islockedForViewing | boolean | indicates whether locks project for viewing. |
| password | string | If the value is null, unprotects this VBA project, otherwise projects the this VBA project. |

**Remarks**

If islockedForViewing is true, the password could not be null.

### copy(VbaProject) {#copy-vbaproject-}

Copy VBA project from other file.

```javascript
copy(source: VbaProject) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [VbaProject](../vbaproject/) |  |

### validatePassword(string) {#validatePassword-string-}

Validates protection password.

```javascript
validatePassword(password: string) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | string | the password |

**Returns**

Whether password is the protection password of this VBA project

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



