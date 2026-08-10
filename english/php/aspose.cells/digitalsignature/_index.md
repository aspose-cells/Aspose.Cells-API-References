---
title: "DigitalSignature Class"
linktitle: "DigitalSignature"
articleTitle: "DigitalSignature"
second_title: "Aspose.Cells for PHP via Java"
description: "Signature in file."
type: docs
weight: 1770
url: /php/aspose.cells/digitalsignature/
---

## DigitalSignature class

Signature in file.

## Constructors

| Name | Description |
| --- | --- |
| [DigitalSignature](#constructor) |  |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Certificate](#certificate) | KeyStore | Certificate object that was used to sign the document. |
| [Comments](#comments) | String | The purpose to signature. |
| [SignTime](#signtime) | DateTime | The time when the document was signed. |
| [Id](#id) | UUID | Specifies a GUID which can be cross-referenced with the GUID of the signature line stored in the document content. Defau |
| [Text](#text) | String | Specifies the text of actual signature in the digital signature. Default value is Empty. |
| [Image](#image) | byte[] | Specifies an image for the digital signature. Default value is null. |
| [ProviderId](#providerid) | UUID | Specifies the class ID of the signature provider. Default value is Empty (all zeroes) Guid. The cryptographic service pr |
| [IsValid](#isvalid) | boolean | If this digital signature is valid and the document has not been tampered with, this value will be true. |
| [XAdESType](#xadestype) | Number | XAdES type. Default value is None(XAdES is off). The value of the property is XAdESType integer constant. |

### DigitalSignature(certificate, privateKeyPassword, comments, signTime) {#constructor}

### DigitalSignature.Certificate property {#certificate}

Certificate object that was used to sign the document.

**Type:** KeyStore

### DigitalSignature.Comments property {#comments}

The purpose to signature.

**Type:** String

### DigitalSignature.SignTime property {#signtime}

The time when the document was signed.

**Type:** DateTime

### DigitalSignature.Id property {#id}

Specifies a GUID which can be cross-referenced with the GUID of the signature line stored in the document content. Default value is Empty (all zeroes) Guid. When set, it associates SignatureLine with corresponding DigitalSignature .

**Type:** UUID

### DigitalSignature.Text property {#text}

Specifies the text of actual signature in the digital signature. Default value is Empty.

**Type:** String

### DigitalSignature.Image property {#image}

Specifies an image for the digital signature. Default value is null.

**Type:** byte[]

### DigitalSignature.ProviderId property {#providerid}

Specifies the class ID of the signature provider. Default value is Empty (all zeroes) Guid. The cryptographic service provider (CSP) is an independent software module that actually performs cryptography algorithms for authentication, encoding, and encryption. Microsoft Office reserves the value of {00000000-0000-0000-0000-000000000000} for its default signature provider, and {000CD6A4-0000-0000-C000-000000000046} for its East Asian signature provider. The GUID of the additionally installed provider should be obtained from the documentation shipped with the provider.

**Type:** UUID

### DigitalSignature.IsValid property {#isvalid}

If this digital signature is valid and the document has not been tampered with, this value will be true.

**Type:** boolean

### DigitalSignature.XAdESType property {#xadestype}

XAdES type. Default value is None(XAdES is off). The value of the property is XAdESType integer constant.

**Type:** Number
