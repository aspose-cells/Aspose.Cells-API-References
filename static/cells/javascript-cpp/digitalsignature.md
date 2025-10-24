##DigitalSignature
Signature in file.
## DigitalSignature class
Signature in file.
```javascript
class DigitalSignature;
```
## Constructors
| Name | Description |
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
