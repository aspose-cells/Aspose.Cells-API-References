---
title: "ReferredArea Klasse"
linktitle: "ReferredArea"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "ReferredArea Klasse. Kapselt das Objekt, das referredarea in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/referredarea/
---

## ReferredArea class

Stellt einen von der Formel referenzierten Bereich dar.

```go

type ReferredArea struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [IsExternalLink](./isexternallink/) | Gibt an, ob dies ein externer Link ist. |
| [GetExternalFileName](./getexternalfilename/) | Liefert den externen Dateinamen, wenn dies eine externe Referenz ist. |
| [GetSheetName](./getsheetname/) | Gibt an, in welchem Blatt sich diese Referenz befindet. |
| [GetSheetNames](./getsheetnames/) | Namen aller Arbeitsblätter, auf die diese Instanz verweist. |
| [IsEntireRow](./isentirerow/) | Gibt an, ob dieser Bereich alle Spalten (ganze Zeile) enthält. |
| [IsEntireColumn](./isentirecolumn/) | Gibt an, ob dieser Bereich alle Zeilen (ganze Spalte) enthält. |
| [IsArea](./isarea/) | Gibt an, ob dies ein Bereich ist. |
| [GetEndColumn](./getendcolumn/) | Die Endspalte des Bereichs. |
| [GetStartColumn](./getstartcolumn/) | Die Startspalte des Bereichs. |
| [GetEndRow](./getendrow/) | Die Endzeile des Bereichs. |
| [GetStartRow](./getstartrow/) | Die Startzeile des Bereichs. |
| [GetValues](./getvalues/) | Ruft Zellwerte in diesem Bereich ab. |
| [GetValues_Bool](./getvalues_bool/) | Ruft Zellwerte in diesem Bereich ab. |
| [GetValue_Int_Int](./getvalue_int_int/) | Ruft den Zellwert mit dem angegebenen Versatz von der oberen linken Ecke dieses Bereichs ab. |
| [GetValue_Int_Int_Bool](./getvalue_int_int_bool/) | Ruft den Zellwert mit dem angegebenen Versatz von der oberen linken Ecke dieses Bereichs ab. |
| [ToString](./tostring/) | Gibt die Referenzadresse dieses Bereichs zurück.Allgemein ist es die Adresse der Referenz, die in einer Formel verwendet werden kann, z. B. "Sheet1!A1:C3". |
