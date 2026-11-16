---
title: "FormulaParseOptions Klasse"
linktitle: "FormulaParseOptions"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "FormulaParseOptions Klasse. Kapselt das Objekt, das formulaparseoptions in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/formulaparseoptions/
---

## FormulaParseOptions class

Stellt Optionen beim Parsen von Formeln dar.

```go

type FormulaParseOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewFormulaParseOptions](./newformulaparseoptions/) | Standardkonstruktor. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetLocaleDependent](./getlocaledependent/) | Ob die Formel lokalspezifisch formatiert ist. Standard ist false. |
| [SetLocaleDependent](./setlocaledependent/) | Ob die Formel lokalspezifisch formatiert ist. Standard ist false. |
| [GetR1C1Style](./getr1c1style/) | Ob die Formel im R1C1-Referenzstil ist. Standard ist false. |
| [SetR1C1Style](./setr1c1style/) | Ob die Formel im R1C1-Referenzstil ist. Standard ist false. |
| [GetCheckAddIn](./getcheckaddin/) | Ob Add‑Ins in bestehenden externen Links der aktuellen Arbeitsmappe für benutzerdefinierte Funktionen ohne externen Link geprüft werden. Standard ist true (wenn die benutzerdefinierte Funktion mit einem Add‑In in bestehenden externen Links übereinstimmt, wird sie als dieses Add‑In behandelt). |
| [SetCheckAddIn](./setcheckaddin/) | Ob Add‑Ins in bestehenden externen Links der aktuellen Arbeitsmappe für benutzerdefinierte Funktionen ohne externen Link geprüft werden. Standard ist true (wenn die benutzerdefinierte Funktion mit einem Add‑In in bestehenden externen Links übereinstimmt, wird sie als dieses Add‑In behandelt). |
| [GetParse](./getparse/) | Ob die gegebene Formel geparst wird. Standard ist true. Ist sie false, bleibt die Formelzeichenkette für die Zelle unverändert, bis der Benutzer andere Methoden aufruft, um sie zu parsen, oder bis geparste Formeldaten von anderen Vorgängen wie der Berechnung von Formeln benötigt werden. |
| [SetParse](./setparse/) | Ob die gegebene Formel geparst wird. Standard ist true. Ist sie false, bleibt die Formelzeichenkette für die Zelle unverändert, bis der Benutzer andere Methoden aufruft, um sie zu parsen, oder bis geparste Formeldaten von anderen Vorgängen wie der Berechnung von Formeln benötigt werden. |
| [GetCustomFunctionDefinition](./getcustomfunctiondefinition/) | Definition zum Parsen benutzerdefinierter Funktionen. |
| [SetCustomFunctionDefinition](./setcustomfunctiondefinition/) | Definition zum Parsen benutzerdefinierter Funktionen. |
