---
title: "DigitalSignature-klass"
linktitle: "DigitalSignature"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "DigitalSignature-klass. Inkapslar objektet som representerar digital signatur i Go."
type: docs
weight: 200
url: /sv/go-cpp/digitalsignature/
---

## DigitalSignature class

Signatur i filen.

```go

type DigitalSignature struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewDigitalSignature_Stream_String_String_Date](./newdigitalsignature_stream_string_string_date/) | Konstruktor för DigitalSignature. |
| [NewDigitalSignature_String_String_String_Date](./newdigitalsignature_string_string_string_date/) | Konstruktor för DigitalSignature. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetComments](./getcomments/) | Syftet med signaturen. |
| [SetComments](./setcomments/) | Syftet med signaturen. |
| [GetSignTime](./getsigntime/) | Tidpunkten då dokumentet signerades. |
| [SetSignTime](./setsigntime/) | Tidpunkten då dokumentet signerades. |
| [GetId](./getid/) | Anger en GUID som kan korsrefereras med GUID för signaturlinjen som lagras i dokumentets innehåll. Standardvärdet är Tom (alla nollor) GUID. |
| [SetId](./setid/) | Anger en GUID som kan korsrefereras med GUID för signaturlinjen som lagras i dokumentets innehåll. Standardvärdet är Tom (alla nollor) GUID. |
| [GetText](./gettext/) | Anger texten för den faktiska signaturen i den digitala signaturen. Standardvärdet är Tom. |
| [SetText](./settext/) | Anger texten för den faktiska signaturen i den digitala signaturen. Standardvärdet är Tom. |
| [GetImage](./getimage/) | Anger en bild för den digitala signaturen. Standardvärdet är null. |
| [SetImage](./setimage/) | Anger en bild för den digitala signaturen. Standardvärdet är null. |
| [GetProviderId](./getproviderid/) | Anger klass-ID för signaturleverantören. Standardvärdet är Tom (alla nollor) GUID. |
| [SetProviderId](./setproviderid/) | Anger klass-ID för signaturleverantören. Standardvärdet är Tom (alla nollor) GUID. |
| [IsValid](./isvalid/) | Om denna digitala signatur är giltig och dokumentet inte har manipulerats, blir värdet true. |
| [GetXAdESType](./getxadestype/) | XAdES-typ. Standardvärdet är Ingen (XAdES är avstängt). |
| [SetXAdESType](./setxadestype/) | XAdES-typ. Standardvärdet är Ingen (XAdES är avstängt). |
