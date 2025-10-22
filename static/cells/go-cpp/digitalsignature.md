##DigitalSignature Class
'DigitalSignature class. Encapsulates the object that represents digitalsignature in Go.'
## DigitalSignature class
Signature in file.
```go
type DigitalSignature struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewDigitalSignature_Stream_String_String_Date](./newdigitalsignature_stream_string_string_date/) | Constructor of DigitalSignature. |
|[NewDigitalSignature_String_String_String_Date](./newdigitalsignature_string_string_string_date/) | Constructor of DigitalSignature. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetComments](./getcomments/) | The purpose to signature. |
|[SetComments](./setcomments/) | The purpose to signature. |
|[GetSignTime](./getsigntime/) | The time when the document was signed. |
|[SetSignTime](./setsigntime/) | The time when the document was signed. |
|[GetId](./getid/) | Specifies a GUID which can be cross-referenced with the GUID of the signature line stored in the document content.Default value is Empty (all zeroes) Guid. |
|[SetId](./setid/) | Specifies a GUID which can be cross-referenced with the GUID of the signature line stored in the document content.Default value is Empty (all zeroes) Guid. |
|[GetText](./gettext/) | Specifies the text of actual signature in the digital signature.Default value is Empty. |
|[SetText](./settext/) | Specifies the text of actual signature in the digital signature.Default value is Empty. |
|[GetImage](./getimage/) | Specifies an image for the digital signature.Default value is null. |
|[SetImage](./setimage/) | Specifies an image for the digital signature.Default value is null. |
|[GetProviderId](./getproviderid/) | Specifies the class ID of the signature provider.Default value is Empty (all zeroes) Guid. |
|[SetProviderId](./setproviderid/) | Specifies the class ID of the signature provider.Default value is Empty (all zeroes) Guid. |
|[IsValid](./isvalid/) | If this digital signature is valid and the document has not been tampered with,this value will be true. |
|[GetXAdESType](./getxadestype/) | XAdES type.Default value is None(XAdES is off). |
|[SetXAdESType](./setxadestype/) | XAdES type.Default value is None(XAdES is off). |
