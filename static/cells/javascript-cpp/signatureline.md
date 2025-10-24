##SignatureLine
Represent the signature line.
## SignatureLine class
Represent the signature line.
```javascript
class SignatureLine;
```
## Constructors
| Name | Description |
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
