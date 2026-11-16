---
title: "DigitalSignature Klasse"
linktitle: "DigitalSignature"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "DigitalSignature Klasse. Kapselt das Objekt, das die digitalsignature in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/digitalsignature/
---

## DigitalSignature class

Signatur in Datei.

```go

type DigitalSignature struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewDigitalSignature_Stream_String_String_Date](./newdigitalsignature_stream_string_string_date/) | Konstruktor von DigitalSignature. |
| [NewDigitalSignature_String_String_String_Date](./newdigitalsignature_string_string_string_date/) | Konstruktor von DigitalSignature. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetComments](./getcomments/) | Der Zweck der Signatur. |
| [SetComments](./setcomments/) | Der Zweck der Signatur. |
| [GetSignTime](./getsigntime/) | Der Zeitpunkt, zu dem das Dokument signiert wurde. |
| [SetSignTime](./setsigntime/) | Der Zeitpunkt, zu dem das Dokument signiert wurde. |
| [GetId](./getid/) | Gibt eine GUID an, die mit der GUID der im Dokumentinhalt gespeicherten Signaturzeile abgeglichen werden kann. Standardwert ist leer (alle Nullen) GUID. |
| [SetId](./setid/) | Gibt eine GUID an, die mit der GUID der im Dokumentinhalt gespeicherten Signaturzeile abgeglichen werden kann. Standardwert ist leer (alle Nullen) GUID. |
| [GetText](./gettext/) | Gibt den Text der tatsächlichen Signatur in der digitalen Signatur an. Standardwert ist leer. |
| [SetText](./settext/) | Gibt den Text der tatsächlichen Signatur in der digitalen Signatur an. Standardwert ist leer. |
| [GetImage](./getimage/) | Gibt ein Bild für die digitale Signatur an. Standardwert ist null. |
| [SetImage](./setimage/) | Gibt ein Bild für die digitale Signatur an. Standardwert ist null. |
| [GetProviderId](./getproviderid/) | Gibt die Klassen-ID des Signaturanbieters an. Standardwert ist leer (alle Nullen) GUID. |
| [SetProviderId](./setproviderid/) | Gibt die Klassen-ID des Signaturanbieters an. Standardwert ist leer (alle Nullen) GUID. |
| [IsValid](./isvalid/) | Wenn diese digitale Signatur gültig ist und das Dokument nicht manipuliert wurde, ist dieser Wert wahr. |
| [GetXAdESType](./getxadestype/) | XAdES-Typ. Standardwert ist Keine (XAdES ist deaktiviert). |
| [SetXAdESType](./setxadestype/) | XAdES-Typ. Standardwert ist Keine (XAdES ist deaktiviert). |
