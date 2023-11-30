---
title: Aspose::Cells::DigitalSignatures::DigitalSignature class
linktitle: DigitalSignature
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::DigitalSignatures::DigitalSignature class. Signature in file in C++.'
type: docs
weight: 100
url: /cpp/aspose.cells.digitalsignatures/digitalsignature/
---
## DigitalSignature class


Signature in file.

```cpp
class DigitalSignature
```

## Methods

| Method | Description |
| --- | --- |
| [DigitalSignature(const Vector \<uint8_t\>\& rawData, const U16String\& password, const U16String\& comments, const Date\& signTime)](./digitalsignature/) | Constructor of digitalSignature. Uses Bouncy Castle implementation. |
| [DigitalSignature(const Vector \<uint8_t\>\& rawData, const char16_t* password, const char16_t* comments, const Date\& signTime)](./digitalsignature/) | Constructor of digitalSignature. Uses Bouncy Castle implementation. |
| [DigitalSignature(DigitalSignature_Impl* impl)](./digitalsignature/) | Constructs from an implementation object. |
| [DigitalSignature(const DigitalSignature\& src)](./digitalsignature/) | Copy constructor. |
| [GetComments()](./getcomments/) | The purpose to signature. |
| [GetImage()](./getimage/) | Specifies an image for the digital signature. Default value is null. |
| [GetSignTime()](./getsigntime/) | The time when the document was signed. |
| [GetText()](./gettext/) | Specifies the text of actual signature in the digital signature. Default value is Empty. |
| [GetXAdESType()](./getxadestype/) | XAdES type. Default value is [None(XAdES is off)](../../aspose.cells/accesscacheoptions/). |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsValid()](./isvalid/) | If this digital signature is valid and the document has not been tampered with, this value will be true. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const DigitalSignature\& src)](./operator_asm/) | operator= |
| [SetComments(const U16String\& value)](./setcomments/) | The purpose to signature. |
| [SetComments(const char16_t* value)](./setcomments/) | The purpose to signature. |
| [SetImage(const Vector \<uint8_t\>\& value)](./setimage/) | Specifies an image for the digital signature. Default value is null. |
| [SetSignTime(const Date\& value)](./setsigntime/) | The time when the document was signed. |
| [SetText(const U16String\& value)](./settext/) | Specifies the text of actual signature in the digital signature. Default value is Empty. |
| [SetText(const char16_t* value)](./settext/) | Specifies the text of actual signature in the digital signature. Default value is Empty. |
| [SetXAdESType(XAdESType value)](./setxadestype/) | XAdES type. Default value is [None(XAdES is off)](../../aspose.cells/accesscacheoptions/). |
| [~DigitalSignature()](./~digitalsignature/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also

* Namespace [Aspose::Cells::DigitalSignatures](../)
* Library [Aspose.Cells for C++](../../)
