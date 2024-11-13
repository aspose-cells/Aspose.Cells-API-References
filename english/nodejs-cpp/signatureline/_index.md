---
title: SignatureLine
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represent the signature line.
type: docs
url: /nodejs-cpp/signatureline/
---

## SignatureLine class

Represent the signature line.

```javascript
class SignatureLine;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getSigner()](#getSigner--)| Gets or sets the signer. |
| [setSigner(string)](#setSigner-string-)| Gets or sets the signer. |
| [getTitle()](#getTitle--)| Gets or sets the title of singer. |
| [setTitle(string)](#setTitle-string-)| Gets or sets the title of singer. |
| [getEmail()](#getEmail--)| Gets or sets the email of singer. |
| [setEmail(string)](#setEmail-string-)| Gets or sets the email of singer. |
| [isLine()](#isLine--)| Indicates whether it is a signature line. |
| [setIsLine(boolean)](#setIsLine-boolean-)| Indicates whether it is a signature line. |
| [getAllowComments()](#getAllowComments--)| Indicates whether comments could be attached. |
| [setAllowComments(boolean)](#setAllowComments-boolean-)| Indicates whether comments could be attached. |
| [getShowSignedDate()](#getShowSignedDate--)| Indicates whether show signed date. |
| [setShowSignedDate(boolean)](#setShowSignedDate-boolean-)| Indicates whether show signed date. |
| [getInstructions()](#getInstructions--)| Gets or sets the text shown to user at signing time. |
| [setInstructions(string)](#setInstructions-string-)| Gets or sets the text shown to user at signing time. |
| [getSignatureLineType()](#getSignatureLineType--)| Gets or sets the signature type. Default - When the default value is set, the corresponding ProviderId value is fixed to {0000000000-0000-0000-0000-0000000000}. Stamp - When the value is Stamp, the corresponding ProviderId value is usually {000CD6A4-0000-0000-C000-000000000046}. Custom - When the value is Custom, the corresponding ProviderId value usually needs to be set by the user. it should be obtained from the documentation shipped with the provider. |
| [setSignatureLineType(SignatureType)](#setSignatureLineType-signaturetype-)| Gets or sets the signature type. Default - When the default value is set, the corresponding ProviderId value is fixed to {0000000000-0000-0000-0000-0000000000}. Stamp - When the value is Stamp, the corresponding ProviderId value is usually {000CD6A4-0000-0000-C000-000000000046}. Custom - When the value is Custom, the corresponding ProviderId value usually needs to be set by the user. it should be obtained from the documentation shipped with the provider. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### getSigner() {#getSigner--}

Gets or sets the signer.

```javascript
getSigner() : string;
```


### setSigner(string) {#setSigner-string-}

Gets or sets the signer.

```javascript
setSigner(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getTitle() {#getTitle--}

Gets or sets the title of singer.

```javascript
getTitle() : string;
```


### setTitle(string) {#setTitle-string-}

Gets or sets the title of singer.

```javascript
setTitle(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getEmail() {#getEmail--}

Gets or sets the email of singer.

```javascript
getEmail() : string;
```


### setEmail(string) {#setEmail-string-}

Gets or sets the email of singer.

```javascript
setEmail(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isLine() {#isLine--}

Indicates whether it is a signature line.

```javascript
isLine() : boolean;
```


### setIsLine(boolean) {#setIsLine-boolean-}

Indicates whether it is a signature line.

```javascript
setIsLine(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAllowComments() {#getAllowComments--}

Indicates whether comments could be attached.

```javascript
getAllowComments() : boolean;
```


### setAllowComments(boolean) {#setAllowComments-boolean-}

Indicates whether comments could be attached.

```javascript
setAllowComments(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowSignedDate() {#getShowSignedDate--}

Indicates whether show signed date.

```javascript
getShowSignedDate() : boolean;
```


### setShowSignedDate(boolean) {#setShowSignedDate-boolean-}

Indicates whether show signed date.

```javascript
setShowSignedDate(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getInstructions() {#getInstructions--}

Gets or sets the text shown to user at signing time.

```javascript
getInstructions() : string;
```


### setInstructions(string) {#setInstructions-string-}

Gets or sets the text shown to user at signing time.

```javascript
setInstructions(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getSignatureLineType() {#getSignatureLineType--}

Gets or sets the signature type. Default - When the default value is set, the corresponding ProviderId value is fixed to {0000000000-0000-0000-0000-0000000000}. Stamp - When the value is Stamp, the corresponding ProviderId value is usually {000CD6A4-0000-0000-C000-000000000046}. Custom - When the value is Custom, the corresponding ProviderId value usually needs to be set by the user. it should be obtained from the documentation shipped with the provider.

```javascript
getSignatureLineType() : SignatureType;
```


**Returns**

[SignatureType](../signaturetype/)

### setSignatureLineType(SignatureType) {#setSignatureLineType-signaturetype-}

Gets or sets the signature type. Default - When the default value is set, the corresponding ProviderId value is fixed to {0000000000-0000-0000-0000-0000000000}. Stamp - When the value is Stamp, the corresponding ProviderId value is usually {000CD6A4-0000-0000-C000-000000000046}. Custom - When the value is Custom, the corresponding ProviderId value usually needs to be set by the user. it should be obtained from the documentation shipped with the provider.

```javascript
setSignatureLineType(value: SignatureType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SignatureType](../signaturetype/) | The value to set. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



