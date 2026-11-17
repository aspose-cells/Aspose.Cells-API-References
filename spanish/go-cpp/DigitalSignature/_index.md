---
title: "Clase DigitalSignature"
linktitle: "DigitalSignature"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase DigitalSignature. Encapsula el objeto que representa DigitalSignature en Go."
type: docs
weight: 200
url: /es/go-cpp/digitalsignature/
---

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
| [NewDigitalSignature_Stream_String_String_Date](./newdigitalsignature_stream_string_string_date/) | Constructor de DigitalSignature. |
| [NewDigitalSignature_String_String_String_Date](./newdigitalsignature_string_string_string_date/) | Constructor de DigitalSignature. |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [GetComments](./getcomments/) | El propósito de la firma. |
| [SetComments](./setcomments/) | El propósito de la firma. |
| [GetSignTime](./getsigntime/) | El tiempo en que el documento fue firmado. |
| [SetSignTime](./setsigntime/) | El tiempo en que el documento fue firmado. |
| [GetId](./getid/) | Especifica un GUID que puede cruzarse con el GUID de la línea de firma almacenada en el contenido del documento. El valor predeterminado es Empty (todos ceros) Guid. |
| [SetId](./setid/) | Especifica un GUID que puede cruzarse con el GUID de la línea de firma almacenada en el contenido del documento. El valor predeterminado es Empty (todos ceros) Guid. |
| [GetText](./gettext/) | Especifica el texto de la firma real en la firma digital. El valor predeterminado es Empty. |
| [SetText](./settext/) | Especifica el texto de la firma real en la firma digital. El valor predeterminado es Empty. |
| [GetImage](./getimage/) | Especifica una imagen para la firma digital. El valor predeterminado es null. |
| [SetImage](./setimage/) | Especifica una imagen para la firma digital. El valor predeterminado es null. |
| [GetProviderId](./getproviderid/) | Especifica el ID de clase del proveedor de firma. El valor predeterminado es Empty (todos ceros) Guid. |
| [SetProviderId](./setproviderid/) | Especifica el ID de clase del proveedor de firma. El valor predeterminado es Empty (todos ceros) Guid. |
| [IsValid](./isvalid/) | Si esta firma digital es válida y el documento no ha sido manipulado, este valor será verdadero. |
| [GetXAdESType](./getxadestype/) | Tipo XAdES. El valor predeterminado es Ninguno (XAdES está desactivado). |
| [SetXAdESType](./setxadestype/) | Tipo XAdES. El valor predeterminado es Ninguno (XAdES está desactivado). |
