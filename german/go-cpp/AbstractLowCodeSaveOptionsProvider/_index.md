---
title: "AbstractLowCodeSaveOptionsProvider-Klasse"
linktitle: "AbstractLowCodeSaveOptionsProvider"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "AbstractLowCodeSaveOptionsProvider-Klasse. Kapselt das Objekt, das abstractlowcodesaveoptionsprovider in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/abstractlowcodesaveoptionsprovider/
---

## AbstractLowCodeSaveOptionsProvider class

Implementierung zur Bereitstellung mehrerer Speicheroptionen für Prozesse, die mehrere Ausgaben erfordern. Zum Beispiel erfordert die <see cref="SpreadsheetSplitter"/>-Funktion mehrere Ziele, um die geteilten Dateien zu speichern.

```go

type AbstractLowCodeSaveOptionsProvider struct  {
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
| [GetSaveOptions](./getsaveoptions/) | Liest die Speicheroptionen, aus denen die Ausgabeeinstellungen für den aktuell geteilten Teil abgerufen werden. Die Rückgabe von null bedeutet, dass der gegebene Teil übersprungen wird. |
| [Finish](./finish/) | Gibt Ressourcen nach der Verarbeitung des aktuell geteilten Teils frei. |
