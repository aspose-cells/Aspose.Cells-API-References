---
title: "DigitalSignature Classe"
linktitle: "DigitalSignature"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "DigitalSignature class. Incapsula l'oggetto che rappresenta digitalsignature in Go."
type: docs
weight: 200
url: /it/go-cpp/digitalsignature/
---

## DigitalSignature class

Firma nel file.

```go

type DigitalSignature struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewDigitalSignature_Stream_String_String_Date](./newdigitalsignature_stream_string_string_date/) | Costruttore di DigitalSignature. |
| [NewDigitalSignature_String_String_String_Date](./newdigitalsignature_string_string_string_date/) | Costruttore di DigitalSignature. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetComments](./getcomments/) | Lo scopo della firma. |
| [SetComments](./setcomments/) | Lo scopo della firma. |
| [GetSignTime](./getsigntime/) | Il momento in cui il documento è stato firmato. |
| [SetSignTime](./setsigntime/) | Il momento in cui il documento è stato firmato. |
| [GetId](./getid/) | Specifica un GUID che può essere incrociato con il GUID della linea di firma memorizzata nel contenuto del documento. Il valore predefinito è Empty (all zeroes) Guid. |
| [SetId](./setid/) | Specifica un GUID che può essere incrociato con il GUID della linea di firma memorizzata nel contenuto del documento. Il valore predefinito è Empty (all zeroes) Guid. |
| [GetText](./gettext/) | Specifica il testo della firma reale nella firma digitale. Il valore predefinito è Empty. |
| [SetText](./settext/) | Specifica il testo della firma reale nella firma digitale. Il valore predefinito è Empty. |
| [GetImage](./getimage/) | Specifica un'immagine per la firma digitale. Il valore predefinito è null. |
| [SetImage](./setimage/) | Specifica un'immagine per la firma digitale. Il valore predefinito è null. |
| [GetProviderId](./getproviderid/) | Specifica l'ID di classe del provider di firma. Il valore predefinito è Empty (all zeroes) Guid. |
| [SetProviderId](./setproviderid/) | Specifica l'ID di classe del provider di firma. Il valore predefinito è Empty (all zeroes) Guid. |
| [IsValid](./isvalid/) | Se questa firma digitale è valida e il documento non è stato manomesso, questo valore sarà vero. |
| [GetXAdESType](./getxadestype/) | Tipo XAdES. Il valore predefinito è Nessuno (XAdES è disattivato). |
| [SetXAdESType](./setxadestype/) | Tipo XAdES. Il valore predefinito è Nessuno (XAdES è disattivato). |
