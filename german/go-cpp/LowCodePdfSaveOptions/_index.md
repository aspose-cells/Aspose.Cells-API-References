---
title: "LowCodePdfSaveOptions Klasse"
linktitle: "LowCodePdfSaveOptions"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "LowCodePdfSaveOptions Klasse. Kapselt das Objekt, das lowcodepdfsaveoptions in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/lowcodepdfsaveoptions/
---

## LowCodePdfSaveOptions class

Optionen zum Speichern von PDF auf Low-Code-Art.

```go

type LowCodePdfSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewLowCodePdfSaveOptions](./newlowcodepdfsaveoptions/) | Standardkonstruktor. |
| [NewLowCodePdfSaveOptions_LowCodeSaveOptions](./newlowcodepdfsaveoptions_lowcodesaveoptions/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetSaveFormat](./getsaveformat/) | Das Speicherformat für die Ausgabe. Beim Konvertieren zu PDF kann es nur SaveFormat.Pdf sein. |
| [SetSaveFormat](./setsaveformat/) | Das Speicherformat für die Ausgabe. Beim Konvertieren zu PDF kann es nur SaveFormat.Pdf sein. |
| [GetPdfOptions](./getpdfoptions/) | Die Optionen zum Speichern der PDF-Datei. |
| [SetPdfOptions](./setpdfoptions/) | Die Optionen zum Speichern der PDF-Datei. |
| [GetOutputFile](./getoutputfile/) | Liest und setzt die Datei (mit Pfad falls nötig) zum Speichern der generierten Daten. Beim Setzen dieser Eigenschaft mit einem Wert, der nicht null oder ein leerer String ist, wird OutputStream ignoriert. |
| [SetOutputFile](./setoutputfile/) | Liest und setzt die Datei (mit Pfad falls nötig) zum Speichern der generierten Daten. Beim Setzen dieser Eigenschaft mit einem Wert, der nicht null oder ein leerer String ist, wird OutputStream ignoriert. |
| [GetOutputStream](./getoutputstream/) | Liest und setzt den Stream zum Schreiben der generierten Daten. Beim Setzen dieser Eigenschaft mit einem Wert, der nicht null ist, wird OutputFile ignoriert. |
| [SetOutputStream](./setoutputstream/) | Liest und setzt den Stream zum Schreiben der generierten Daten. Beim Setzen dieser Eigenschaft mit einem Wert, der nicht null ist, wird OutputFile ignoriert. |
