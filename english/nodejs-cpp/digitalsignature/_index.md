---
title: DigitalSignature
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Signature in file.
type: docs
url: /nodejs-cpp/digitalsignature/
---

## DigitalSignature class

Signature in file.

```javascript
class DigitalSignature;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(number[], string, string, Date)](#constructor-numberarray-string-string-date-)| Constructor of DigitalSignature. |
| [constructor(string, string, string, Date)](#constructor-string-string-string-date-)| Constructor of DigitalSignature. |

## Methods

| Method | Description |
| --- | --- |
| [getComments()](#getComments--)| The purpose to signature. |
| [setComments(string)](#setComments-string-)| The purpose to signature. |
| [getSignTime()](#getSignTime--)| The time when the document was signed. |
| [setSignTime(Date)](#setSignTime-date-)| The time when the document was signed. |
| [getText()](#getText--)| Specifies the text of actual signature in the digital signature. Default value is Empty. |
| [setText(string)](#setText-string-)| Specifies the text of actual signature in the digital signature. Default value is Empty. |
| [getImage()](#getImage--)| Specifies an image for the digital signature. Default value is null. |
| [setImage(number[])](#setImage-numberarray-)| Specifies an image for the digital signature. Default value is null. |
| [isValid()](#isValid--)| If this digital signature is valid and the document has not been tampered with, this value will be true. |
| [getXAdESType()](#getXAdESType--)| XAdES type. Default value is None(XAdES is off). |
| [setXAdESType(XAdESType)](#setXAdESType-xadestype-)| XAdES type. Default value is None(XAdES is off). |


### constructor(number[], string, string, Date) {#constructor-numberarray-string-string-date-}

Constructor of DigitalSignature.

```javascript
constructor(rawData: number[], password: string, comments: string, signTime: Date);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rawData | number[] | A byte array containing data from an X.509 certificate. |
| password | string | The password required to access the X.509 certificate data. |
| comments | string | The purpose to signature. |
| signTime | Date | The utc time when the document was signed. |

### constructor(string, string, string, Date) {#constructor-string-string-string-date-}

Constructor of DigitalSignature.

```javascript
constructor(fileName: string, password: string, comments: string, signTime: Date);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | string | The name of a certificate file. |
| password | string | The password required to access the X.509 certificate data. |
| comments | string | The purpose to signature. |
| signTime | Date | The utc time when the document was signed. |

### getComments() {#getComments--}

The purpose to signature.

```javascript
getComments() : string;
```


### setComments(string) {#setComments-string-}

The purpose to signature.

```javascript
setComments(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getSignTime() {#getSignTime--}

The time when the document was signed.

```javascript
getSignTime() : Date;
```


### setSignTime(Date) {#setSignTime-date-}

The time when the document was signed.

```javascript
setSignTime(value: Date) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Date | The value to set. |

### getText() {#getText--}

Specifies the text of actual signature in the digital signature. Default value is Empty.

```javascript
getText() : string;
```


### setText(string) {#setText-string-}

Specifies the text of actual signature in the digital signature. Default value is Empty.

```javascript
setText(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getImage() {#getImage--}

Specifies an image for the digital signature. Default value is null.

```javascript
getImage() : number[];
```


**Returns**

number[]

### setImage(number[]) {#setImage-numberarray-}

Specifies an image for the digital signature. Default value is null.

```javascript
setImage(value: number[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |

### isValid() {#isValid--}

If this digital signature is valid and the document has not been tampered with, this value will be true.

```javascript
isValid() : boolean;
```


### getXAdESType() {#getXAdESType--}

XAdES type. Default value is None(XAdES is off).

```javascript
getXAdESType() : XAdESType;
```


**Returns**

[XAdESType](../xadestype/)

### setXAdESType(XAdESType) {#setXAdESType-xadestype-}

XAdES type. Default value is None(XAdES is off).

```javascript
setXAdESType(value: XAdESType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [XAdESType](../xadestype/) | The value to set. |


