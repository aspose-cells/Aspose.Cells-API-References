---
title: "VbaProject Klasse"
linktitle: "VbaProject"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "VbaProject Klasse. Kapselt das Objekt, das vbaproject in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/vbaproject/
---

## VbaProject class

Stellt das VBA-Projekt dar.

```go

type VbaProject struct  {
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
| [Sign](./sign/) | Signiere dieses VBA-Projekt mit einer DigitalSignature |
| [IsValidSigned](./isvalidsigned/) | Gibt an, ob die Signatur des VBA-Projekts gültig ist oder nicht. |
| [GetCertRawData](./getcertrawdata/) | Liest die rohen Zertifikatsdaten, wenn dieses VBA-Projekt signiert ist. |
| [GetEncoding](./getencoding/) | Liest und setzt die Kodierung des VBA-Projekts. |
| [SetEncoding](./setencoding/) | Liest und setzt die Kodierung des VBA-Projekts. |
| [GetName](./getname/) | Liest und setzt den Namen des VBA-Projekts. |
| [SetName](./setname/) | Liest und setzt den Namen des VBA-Projekts. |
| [IsSigned](./issigned/) | Gibt an, ob VBAcode signiert ist oder nicht. |
| [Protect](./protect/) | Schützt oder hebt den Schutz dieses VBA-Projekts auf. |
| [IsProtected](./isprotected/) | Gibt an, ob dieses VBA-Projekt geschützt ist. |
| [IsLockedForView](./islockedforview/) | Gibt an, ob dieses VBA-Projekt für die Ansicht gesperrt ist. Wenn true, können die Codes nicht angezeigt werden. |
| [Copy](./copy/) | VBA-Projekt aus einer anderen Datei kopieren. |
| [GetModules](./getmodules/) | Liefert alle VbaModule-Objekte. |
| [GetReferences](./getreferences/) | Liefert alle Verweise des VBA-Projekts. |
| [ValidatePassword](./validatepassword/) | Validiert das Schutzkennwort. |
