---
title: "SignatureLine Klasse"
linktitle: "SignatureLine"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "SignatureLine Klasse. Kapselt das Objekt, das signatureline in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/signatureline/
---

## SignatureLine class

Stellt die Signaturzeile dar.

```go

type SignatureLine struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewSignatureLine](./newsignatureline/) | Standardkonstruktor. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetId](./getid/) | Liest oder setzt den Bezeichner für diese Signaturzeile. |
| [SetId](./setid/) | Liest oder setzt den Bezeichner für diese Signaturzeile. |
| [GetProviderId](./getproviderid/) | Liest oder setzt die ID des Signaturanbieters. |
| [SetProviderId](./setproviderid/) | Liest oder setzt die ID des Signaturanbieters. |
| [GetSigner](./getsigner/) | Liest oder setzt den Unterzeichner. |
| [SetSigner](./setsigner/) | Liest oder setzt den Unterzeichner. |
| [GetTitle](./gettitle/) | Liest oder setzt den Titel des Unterzeichners. |
| [SetTitle](./settitle/) | Liest oder setzt den Titel des Unterzeichners. |
| [GetEmail](./getemail/) | Liest oder setzt die E‑Mail des Unterzeichners. |
| [SetEmail](./setemail/) | Liest oder setzt die E‑Mail des Unterzeichners. |
| [IsLine](./isline/) | Gibt an, ob es eine Signaturzeile ist. |
| [SetIsLine](./setisline/) | Gibt an, ob es eine Signaturzeile ist. |
| [GetAllowComments](./getallowcomments/) | Gibt an, ob Kommentare angehängt werden können. |
| [SetAllowComments](./setallowcomments/) | Gibt an, ob Kommentare angehängt werden können. |
| [GetShowSignedDate](./getshowsigneddate/) | Gibt an, ob das Unterzeichnungsdatum angezeigt wird. |
| [SetShowSignedDate](./setshowsigneddate/) | Gibt an, ob das Unterzeichnungsdatum angezeigt wird. |
| [GetInstructions](./getinstructions/) | Liest oder setzt den Text, der dem Benutzer beim Signieren angezeigt wird. |
| [SetInstructions](./setinstructions/) | Liest oder setzt den Text, der dem Benutzer beim Signieren angezeigt wird. |
| [GetSignatureLineType](./getsignaturelinetype/) | Liest oder setzt den Signaturtyp. Default - Wenn der Standardwert gesetzt ist, ist der entsprechende ProviderId‑Wert fest auf {0000000000-0000-0000-0000-0000000000}. Stamp - Wenn der Wert Stamp ist, ist der entsprechende ProviderId‑Wert normalerweise {000CD6A4-0000-0000-C000-000000000046}. Custom - Wenn der Wert Custom ist, muss der entsprechende ProviderId‑Wert in der Regel vom Benutzer gesetzt werden. Er sollte aus der Dokumentation des Anbieters entnommen werden. |
| [SetSignatureLineType](./setsignaturelinetype/) | Liest oder setzt den Signaturtyp. Default - Wenn der Standardwert gesetzt ist, ist der entsprechende ProviderId‑Wert fest auf {0000000000-0000-0000-0000-0000000000}. Stamp - Wenn der Wert Stamp ist, ist der entsprechende ProviderId‑Wert normalerweise {000CD6A4-0000-0000-C000-000000000046}. Custom - Wenn der Wert Custom ist, muss der entsprechende ProviderId‑Wert in der Regel vom Benutzer gesetzt werden. Er sollte aus der Dokumentation des Anbieters entnommen werden. |
