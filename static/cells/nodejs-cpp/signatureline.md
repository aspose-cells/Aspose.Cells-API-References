##SignatureLine
Represent the signature line.
## SignatureLine class
Represent the signature line.
```javascript
class SignatureLine;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [signer](#signer--)| string | Gets or sets the signer. |
| [title](#title--)| string | Gets or sets the title of singer. |
| [email](#email--)| string | Gets or sets the email of singer. |
| [isLine](#isLine--)| boolean | Indicates whether it is a signature line. |
| [allowComments](#allowComments--)| boolean | Indicates whether comments could be attached. |
| [showSignedDate](#showSignedDate--)| boolean | Indicates whether show signed date. |
| [instructions](#instructions--)| string | Gets or sets the text shown to user at signing time. |
| [signatureLineType](#signatureLineType--)| SignatureType | Gets or sets the signature type. Default - When the default value is set, the corresponding ProviderId value is fixed to {0000000000-0000-0000-0000-0000000000}. Stamp - When the value is Stamp, the corresponding ProviderId value is usually {000CD6A4-0000-0000-C000-000000000046}. Custom - When the value is Custom, the corresponding ProviderId value usually needs to be set by the user. it should be obtained from the documentation shipped with the provider. |
## Methods
| Method | Description |
| --- | --- |
| [getSigner()](#getSigner--)| <b>@deprecated.</b> Please use the 'signer' property instead. Gets or sets the signer. |
| [setSigner(string)](#setSigner-string-)| <b>@deprecated.</b> Please use the 'signer' property instead. Gets or sets the signer. |
| [getTitle()](#getTitle--)| <b>@deprecated.</b> Please use the 'title' property instead. Gets or sets the title of singer. |
| [setTitle(string)](#setTitle-string-)| <b>@deprecated.</b> Please use the 'title' property instead. Gets or sets the title of singer. |
| [getEmail()](#getEmail--)| <b>@deprecated.</b> Please use the 'email' property instead. Gets or sets the email of singer. |
| [setEmail(string)](#setEmail-string-)| <b>@deprecated.</b> Please use the 'email' property instead. Gets or sets the email of singer. |
| [isLine()](#isLine--)| <b>@deprecated.</b> Please use the 'isLine' property instead. Indicates whether it is a signature line. |
| [setIsLine(boolean)](#setIsLine-boolean-)| <b>@deprecated.</b> Please use the 'isLine' property instead. Indicates whether it is a signature line. |
| [getAllowComments()](#getAllowComments--)| <b>@deprecated.</b> Please use the 'allowComments' property instead. Indicates whether comments could be attached. |
| [setAllowComments(boolean)](#setAllowComments-boolean-)| <b>@deprecated.</b> Please use the 'allowComments' property instead. Indicates whether comments could be attached. |
| [getShowSignedDate()](#getShowSignedDate--)| <b>@deprecated.</b> Please use the 'showSignedDate' property instead. Indicates whether show signed date. |
| [setShowSignedDate(boolean)](#setShowSignedDate-boolean-)| <b>@deprecated.</b> Please use the 'showSignedDate' property instead. Indicates whether show signed date. |
| [getInstructions()](#getInstructions--)| <b>@deprecated.</b> Please use the 'instructions' property instead. Gets or sets the text shown to user at signing time. |
| [setInstructions(string)](#setInstructions-string-)| <b>@deprecated.</b> Please use the 'instructions' property instead. Gets or sets the text shown to user at signing time. |
| [getSignatureLineType()](#getSignatureLineType--)| <b>@deprecated.</b> Please use the 'signatureLineType' property instead. Gets or sets the signature type. Default - When the default value is set, the corresponding ProviderId value is fixed to {0000000000-0000-0000-0000-0000000000}. Stamp - When the value is Stamp, the corresponding ProviderId value is usually {000CD6A4-0000-0000-C000-000000000046}. Custom - When the value is Custom, the corresponding ProviderId value usually needs to be set by the user. it should be obtained from the documentation shipped with the provider. |
| [setSignatureLineType(SignatureType)](#setSignatureLineType-signaturetype-)| <b>@deprecated.</b> Please use the 'signatureLineType' property instead. Gets or sets the signature type. Default - When the default value is set, the corresponding ProviderId value is fixed to {0000000000-0000-0000-0000-0000000000}. Stamp - When the value is Stamp, the corresponding ProviderId value is usually {000CD6A4-0000-0000-C000-000000000046}. Custom - When the value is Custom, the corresponding ProviderId value usually needs to be set by the user. it should be obtained from the documentation shipped with the provider. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### signer {#signer--}
Gets or sets the signer.
```javascript
signer : string;
```
### title {#title--}
Gets or sets the title of singer.
```javascript
title : string;
```
### email {#email--}
Gets or sets the email of singer.
```javascript
email : string;
```
### isLine {#isLine--}
Indicates whether it is a signature line.
```javascript
isLine : boolean;
```
### allowComments {#allowComments--}
Indicates whether comments could be attached.
```javascript
allowComments : boolean;
```
### showSignedDate {#showSignedDate--}
Indicates whether show signed date.
```javascript
showSignedDate : boolean;
```
### instructions {#instructions--}
Gets or sets the text shown to user at signing time.
```javascript
instructions : string;
```
### signatureLineType {#signatureLineType--}
Gets or sets the signature type. Default - When the default value is set, the corresponding ProviderId value is fixed to {0000000000-0000-0000-0000-0000000000}. Stamp - When the value is Stamp, the corresponding ProviderId value is usually {000CD6A4-0000-0000-C000-000000000046}. Custom - When the value is Custom, the corresponding ProviderId value usually needs to be set by the user. it should be obtained from the documentation shipped with the provider.
```javascript
signatureLineType : SignatureType;
```
### getSigner() {#getSigner--}
```javascript
getSigner() : string;
```
### setSigner(string) {#setSigner-string-}
```javascript
setSigner(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getTitle() {#getTitle--}
```javascript
getTitle() : string;
```
### setTitle(string) {#setTitle-string-}
```javascript
setTitle(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getEmail() {#getEmail--}
```javascript
getEmail() : string;
```
### setEmail(string) {#setEmail-string-}
```javascript
setEmail(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### isLine() {#isLine--}
```javascript
isLine() : boolean;
```
### setIsLine(boolean) {#setIsLine-boolean-}
```javascript
setIsLine(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAllowComments() {#getAllowComments--}
```javascript
getAllowComments() : boolean;
```
### setAllowComments(boolean) {#setAllowComments-boolean-}
```javascript
setAllowComments(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowSignedDate() {#getShowSignedDate--}
```javascript
getShowSignedDate() : boolean;
```
### setShowSignedDate(boolean) {#setShowSignedDate-boolean-}
```javascript
setShowSignedDate(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getInstructions() {#getInstructions--}
```javascript
getInstructions() : string;
```
### setInstructions(string) {#setInstructions-string-}
```javascript
setInstructions(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getSignatureLineType() {#getSignatureLineType--}
```javascript
getSignatureLineType() : SignatureType;
```
**Returns**
[SignatureType](../signaturetype/)
### setSignatureLineType(SignatureType) {#setSignatureLineType-signaturetype-}
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
