---
title: "DigitalSignature"
linktitle: "DigitalSignature"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Signature in file."
type: docs
weight: 1180
url: /nodejs/aspose.cells/digitalsignature/
---

## DigitalSignature class

Signature in file.

```js
new DigitalSignature()
```

## Methods

| Name | Description |
| --- | --- |
| [getCertificate()](#getcertificate) | Certificate object that was used to sign the document. |
| [getComments()](#getcomments) | The purpose to signature. |
| [getId()](#getid) | Specifies a GUID which can be cross-referenced with the GUID of the signature line stored in the document content. Defau |
| [getImage()](#getimage) | Specifies an image for the digital signature. Default value is null. |
| [getProviderId()](#getproviderid) | Specifies the class ID of the signature provider. Default value is Empty (all zeroes) Guid. The cryptographic service pr |
| [getSignTime()](#getsigntime) | The time when the document was signed. |
| [getText()](#gettext) | Specifies the text of actual signature in the digital signature. Default value is Empty. |
| [getXAdESType()](#getxadestype) | XAdES type. Default value is None(XAdES is off). The value of the property is XAdESType integer constant. |
| [isValid()](#isvalid) | If this digital signature is valid and the document has not been tampered with, this value will be true. |
| [setCertificate()](#setcertificate) | Certificate object that was used to sign the document. |
| [setComments()](#setcomments) | The purpose to signature. |
| [setId()](#setid) | Specifies a GUID which can be cross-referenced with the GUID of the signature line stored in the document content. Defau |
| [setImage()](#setimage) | Specifies an image for the digital signature. Default value is null. |
| [setProviderId()](#setproviderid) | Specifies the class ID of the signature provider. Default value is Empty (all zeroes) Guid. The cryptographic service pr |
| [setSignTime()](#setsigntime) | The time when the document was signed. |
| [setText()](#settext) | Specifies the text of actual signature in the digital signature. Default value is Empty. |
| [setXAdESType()](#setxadestype) | XAdES type. Default value is None(XAdES is off). The value of the property is XAdESType integer constant. |

### getCertificate() {#getcertificate}

Certificate object that was used to sign the document.

### getComments() {#getcomments}

The purpose to signature.

### getId() {#getid}

Specifies a GUID which can be cross-referenced with the GUID of the signature line stored in the document content. Default value is Empty (all zeroes) Guid. When set, it associates SignatureLine with corresponding DigitalSignature.

### getImage() {#getimage}

Specifies an image for the digital signature. Default value is null.

### getProviderId() {#getproviderid}

Specifies the class ID of the signature provider. Default value is Empty (all zeroes) Guid. The cryptographic service provider (CSP) is an independent software module that actually performs cryptography algorithms for authentication, encoding, and encryption. Microsoft Office reserves the value of {00000000-0000-0000-0000-000000000000} for its default signature provider, and {000CD6A4-0000-0000-C000-000000000046} for its East Asian signature provider. The GUID of the additionally installed provider should be obtained from the documentation shipped with the provider.

### getSignTime() {#getsigntime}

The time when the document was signed.

### getText() {#gettext}

Specifies the text of actual signature in the digital signature. Default value is Empty.

### getXAdESType() {#getxadestype}

XAdES type. Default value is None(XAdES is off). The value of the property is XAdESType integer constant.

### isValid() {#isvalid}

If this digital signature is valid and the document has not been tampered with, this value will be true.

### setCertificate() {#setcertificate}

Certificate object that was used to sign the document.

### setComments() {#setcomments}

The purpose to signature.

### setId() {#setid}

Specifies a GUID which can be cross-referenced with the GUID of the signature line stored in the document content. Default value is Empty (all zeroes) Guid. When set, it associates SignatureLine with corresponding DigitalSignature.

### setImage() {#setimage}

Specifies an image for the digital signature. Default value is null.

### setProviderId() {#setproviderid}

Specifies the class ID of the signature provider. Default value is Empty (all zeroes) Guid. The cryptographic service provider (CSP) is an independent software module that actually performs cryptography algorithms for authentication, encoding, and encryption. Microsoft Office reserves the value of {00000000-0000-0000-0000-000000000000} for its default signature provider, and {000CD6A4-0000-0000-C000-000000000046} for its East Asian signature provider. The GUID of the additionally installed provider should be obtained from the documentation shipped with the provider.

### setSignTime() {#setsigntime}

The time when the document was signed.

### setText() {#settext}

Specifies the text of actual signature in the digital signature. Default value is Empty.

### setXAdESType() {#setxadestype}

XAdES type. Default value is None(XAdES is off). The value of the property is XAdESType integer constant.
