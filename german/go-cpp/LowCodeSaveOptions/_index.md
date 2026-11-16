---
title: "LowCodeSaveOptions Klasse"
linktitle: "LowCodeSaveOptions"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "LowCodeSaveOptions Klasse. Kapselt das Objekt, das lowcodesaveoptions in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/lowcodesaveoptions/
---

## LowCodeSaveOptions class

Optionen zum Speichern generierter Ergebnisse auf Low-Code-Art.

```go

type LowCodeSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewLowCodeSaveOptions](./newlowcodesaveoptions/) | Standardkonstruktor. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetOutputFile](./getoutputfile/) | Liest und setzt die Datei (mit Pfad falls nötig) zum Speichern der generierten Daten. Beim Setzen dieser Eigenschaft mit einem Wert, der nicht null oder ein leerer String ist, wird OutputStream ignoriert. |
| [SetOutputFile](./setoutputfile/) | Liest und setzt die Datei (mit Pfad falls nötig) zum Speichern der generierten Daten. Beim Setzen dieser Eigenschaft mit einem Wert, der nicht null oder ein leerer String ist, wird OutputStream ignoriert. |
| [GetOutputStream](./getoutputstream/) | Liest und setzt den Stream zum Schreiben der generierten Daten. Beim Setzen dieser Eigenschaft mit einem Wert, der nicht null ist, wird OutputFile ignoriert. |
| [SetOutputStream](./setoutputstream/) | Liest und setzt den Stream zum Schreiben der generierten Daten. Beim Setzen dieser Eigenschaft mit einem Wert, der nicht null ist, wird OutputFile ignoriert. |
| [GetSaveFormat](./getsaveformat/) | Liest und schreibt das Speicherformat für die Ausgabe.Im Allgemeinen sind für einen spezifischen Prozess im Low‑Code‑Modus nur bestimmte Formate zulässig.Bitte geben Sie das korrekte Format für den entsprechenden Prozess an, sonst kann ein unerwartetes Ergebnis oder sogar eine Ausnahme auftreten. |
| [SetSaveFormat](./setsaveformat/) | Liest und schreibt das Speicherformat für die Ausgabe.Im Allgemeinen sind für einen spezifischen Prozess im Low‑Code‑Modus nur bestimmte Formate zulässig.Bitte geben Sie das korrekte Format für den entsprechenden Prozess an, sonst kann ein unerwartetes Ergebnis oder sogar eine Ausnahme auftreten. |
