##Aspose::Cells::DigitalSignatures::DigitalSignature class
'Aspose::Cells::DigitalSignatures::DigitalSignature class. Signature in file in C++.'
## DigitalSignature class
Signature in file.
```cpp
class DigitalSignature
```
## Methods
| Method | Description |
| --- | --- |
| [DigitalSignature(const Vector \<uint8_t\>\& rawData, const U16String\& password, const U16String\& comments, const Date\& signTime)](./digitalsignature/) | Constructor of [DigitalSignature](./). |
| [DigitalSignature(const Vector \<uint8_t\>\& rawData, const char16_t* password, const char16_t* comments, const Date\& signTime)](./digitalsignature/) | Constructor of [DigitalSignature](./). |
| [DigitalSignature(const U16String\& fileName, const U16String\& password, const U16String\& comments, const Date\& signTime)](./digitalsignature/) | Constructor of [DigitalSignature](./). |
| [DigitalSignature(const char16_t* fileName, const char16_t* password, const char16_t* comments, const Date\& signTime)](./digitalsignature/) | Constructor of [DigitalSignature](./). |
| [DigitalSignature(DigitalSignature_Impl* impl)](./digitalsignature/) | Constructs from an implementation object. |
| [DigitalSignature(const DigitalSignature\& src)](./digitalsignature/) | Copy constructor. |
| [GetComments()](./getcomments/) | The purpose to signature. |
| [GetId(UUID\& uuid)](./getid/) | Specifies a GUID which can be cross-referenced with the GUID of the signature line stored in the document content. Default value is Empty (all zeroes) Guid. |
| [GetImage()](./getimage/) | Specifies an image for the digital signature. Default value is null. |
| [GetProviderId(UUID\& uuid)](./getproviderid/) | Specifies the class ID of the signature provider. Default value is Empty (all zeroes) Guid. |
| [GetSignTime()](./getsigntime/) | The time when the document was signed. |
| [GetText()](./gettext/) | Specifies the text of actual signature in the digital signature. Default value is Empty. |
| [GetXAdESType()](./getxadestype/) | XAdES type. Default value is [None(XAdES is off)](../../aspose.cells/accesscacheoptions/). |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsValid()](./isvalid/) | If this digital signature is valid and the document has not been tampered with, this value will be true. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const DigitalSignature\& src)](./operator_asm/) | operator= |
| [SetComments(const U16String\& value)](./setcomments/) | The purpose to signature. |
| [SetComments(const char16_t* value)](./setcomments/) | The purpose to signature. |
| [SetId(const UUID\& value)](./setid/) | Specifies a GUID which can be cross-referenced with the GUID of the signature line stored in the document content. Default value is Empty (all zeroes) Guid. |
| [SetImage(const Vector \<uint8_t\>\& value)](./setimage/) | Specifies an image for the digital signature. Default value is null. |
| [SetProviderId(const UUID\& value)](./setproviderid/) | Specifies the class ID of the signature provider. Default value is Empty (all zeroes) Guid. |
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
