##DigitalSignature
Signature in file.
## DigitalSignature class
Signature in file.
```javascript
class DigitalSignature;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(Uint8Array, string, string, Date)](#constructor-uint8array-string-string-date-)| Constructor of DigitalSignature. |
| [constructor(string, string, string, Date)](#constructor-string-string-string-date-)| Constructor of DigitalSignature. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [comments](#comments--)| string | The purpose to signature. |
| [signTime](#signTime--)| Date | The time when the document was signed. |
| [text](#text--)| string | Specifies the text of actual signature in the digital signature. Default value is Empty. |
| [image](#image--)| Uint8Array | Specifies an image for the digital signature. Default value is null. |
| [isValid](#isValid--)| boolean | Readonly. If this digital signature is valid and the document has not been tampered with, this value will be true. |
| [xAdESType](#xAdESType--)| XAdESType | XAdES type. Default value is None(XAdES is off). |
## Methods
| Method | Description |
| --- | --- |
| [getComments()](#getComments--)| <b>@deprecated.</b> Please use the 'comments' property instead. The purpose to signature. |
| [setComments(string)](#setComments-string-)| <b>@deprecated.</b> Please use the 'comments' property instead. The purpose to signature. |
| [getSignTime()](#getSignTime--)| <b>@deprecated.</b> Please use the 'signTime' property instead. The time when the document was signed. |
| [setSignTime(Date)](#setSignTime-date-)| <b>@deprecated.</b> Please use the 'signTime' property instead. The time when the document was signed. |
| [getText()](#getText--)| <b>@deprecated.</b> Please use the 'text' property instead. Specifies the text of actual signature in the digital signature. Default value is Empty. |
| [setText(string)](#setText-string-)| <b>@deprecated.</b> Please use the 'text' property instead. Specifies the text of actual signature in the digital signature. Default value is Empty. |
| [getImage()](#getImage--)| <b>@deprecated.</b> Please use the 'image' property instead. Specifies an image for the digital signature. Default value is null. |
| [setImage(Uint8Array)](#setImage-uint8array-)| <b>@deprecated.</b> Please use the 'image' property instead. Specifies an image for the digital signature. Default value is null. |
| [isValid()](#isValid--)| <b>@deprecated.</b> Please use the 'isValid' property instead. If this digital signature is valid and the document has not been tampered with, this value will be true. |
| [getXAdESType()](#getXAdESType--)| <b>@deprecated.</b> Please use the 'xAdESType' property instead. XAdES type. Default value is None(XAdES is off). |
| [setXAdESType(XAdESType)](#setXAdESType-xadestype-)| <b>@deprecated.</b> Please use the 'xAdESType' property instead. XAdES type. Default value is None(XAdES is off). |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor(Uint8Array, string, string, Date) {#constructor-uint8array-string-string-date-}
Constructor of DigitalSignature.
```javascript
constructor(rawData: Uint8Array, password: string, comments: string, signTime: Date);
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
### comments {#comments--}
The purpose to signature.
```javascript
comments : string;
```
### signTime {#signTime--}
The time when the document was signed.
```javascript
signTime : Date;
```
### text {#text--}
Specifies the text of actual signature in the digital signature. Default value is Empty.
```javascript
text : string;
```
### image {#image--}
Specifies an image for the digital signature. Default value is null.
```javascript
image : Uint8Array;
```
### isValid {#isValid--}
Readonly. If this digital signature is valid and the document has not been tampered with, this value will be true.
```javascript
isValid : boolean;
```
### xAdESType {#xAdESType--}
XAdES type. Default value is None(XAdES is off).
```javascript
xAdESType : XAdESType;
```
### getComments() {#getComments--}
```javascript
getComments() : string;
```
### setComments(string) {#setComments-string-}
```javascript
setComments(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getSignTime() {#getSignTime--}
```javascript
getSignTime() : Date;
```
### setSignTime(Date) {#setSignTime-date-}
```javascript
setSignTime(value: Date) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Date | The value to set. |
### getText() {#getText--}
```javascript
getText() : string;
```
### setText(string) {#setText-string-}
```javascript
setText(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getImage() {#getImage--}
```javascript
getImage() : Uint8Array;
```
### setImage(Uint8Array) {#setImage-uint8array-}
```javascript
setImage(value: Uint8Array) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |
### isValid() {#isValid--}
```javascript
isValid() : boolean;
```
### getXAdESType() {#getXAdESType--}
```javascript
getXAdESType() : XAdESType;
```
**Returns**
[XAdESType](../xadestype/)
### setXAdESType(XAdESType) {#setXAdESType-xadestype-}
```javascript
setXAdESType(value: XAdESType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [XAdESType](../xadestype/) | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
