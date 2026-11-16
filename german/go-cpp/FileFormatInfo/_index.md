---
title: "FileFormatInfo Klasse"
linktitle: "FileFormatInfo"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "FileFormatInfo-Klasse. Kapselt das Objekt, das FileFormatInfo in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/fileformatinfo/
---

## FileFormatInfo class

Enthält Daten, die von den Dateiformat‑Erkennungsmethoden <see cref=\"FileFormatUtil\"/> zurückgegeben werden.

```go

type FileFormatInfo struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewFileFormatInfo](./newfileformatinfo/) | Standardkonstruktor. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [IsProtectedByRMS](./isprotectedbyrms/) | Gibt an, ob die Datei durch den Microsoft Rights Management Server geschützt ist. |
| [IsEncrypted](./isencrypted/) | Gibt true zurück, wenn das Dokument verschlüsselt ist und ein Passwort zum Öffnen benötigt. |
| [GetFileFormatType](./getfileformattype/) | Ermittelt das erkannte Dateiformat. |
| [GetLoadFormat](./getloadformat/) | Ermittelt das erkannte Ladeformat. |
