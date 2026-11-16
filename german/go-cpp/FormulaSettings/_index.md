---
title: "FormulaSettings-Klasse"
linktitle: "FormulaSettings"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "FormulaSettings‑Klasse. Kapselt das Objekt, das formulasettings in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/formulasettings/
---

## FormulaSettings class

Einstellungen für Formeln und Berechnungen.

```go

type FormulaSettings struct  {
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
| [GetCalculateOnOpen](./getcalculateonopen/) | Gibt an, ob die Anwendung beim Öffnen der Arbeitsmappe eine vollständige Berechnung durchführen muss. |
| [SetCalculateOnOpen](./setcalculateonopen/) | Gibt an, ob die Anwendung beim Öffnen der Arbeitsmappe eine vollständige Berechnung durchführen muss. |
| [GetCalculateOnSave](./getcalculateonsave/) | Gibt an, ob die Arbeitsmappe im manuellen Berechnungsmodus vor dem Speichern des Dokuments neu berechnet werden soll. |
| [SetCalculateOnSave](./setcalculateonsave/) | Gibt an, ob die Arbeitsmappe im manuellen Berechnungsmodus vor dem Speichern des Dokuments neu berechnet werden soll. |
| [GetForceFullCalculation](./getforcefullcalculation/) | Gibt an, ob bei jeder Auslösung einer Berechnung alle Formeln neu berechnet werden. |
| [SetForceFullCalculation](./setforcefullcalculation/) | Gibt an, ob bei jeder Auslösung einer Berechnung alle Formeln neu berechnet werden. |
| [GetCalculationMode](./getcalculationmode/) | Liest oder setzt den Modus für die Arbeitsmappenberechnung in MS Excel. |
| [SetCalculationMode](./setcalculationmode/) | Liest oder setzt den Modus für die Arbeitsmappenberechnung in MS Excel. |
| [GetCalculationId](./getcalculationid/) | Gibt die Version der Berechnungs-Engine an, die zur Berechnung von Werten in der Arbeitsmappe verwendet wird. |
| [SetCalculationId](./setcalculationid/) | Gibt die Version der Berechnungs-Engine an, die zur Berechnung von Werten in der Arbeitsmappe verwendet wird. |
| [GetEnableIterativeCalculation](./getenableiterativecalculation/) | Gibt an, ob iterative Berechnungen zur Auflösung zirkulärer Verweise aktiviert werden sollen. |
| [SetEnableIterativeCalculation](./setenableiterativecalculation/) | Gibt an, ob iterative Berechnungen zur Auflösung zirkulärer Verweise aktiviert werden sollen. |
| [GetMaxIteration](./getmaxiteration/) | Die maximale Anzahl von Iterationen zur Auflösung eines zirkulären Verweises. |
| [SetMaxIteration](./setmaxiteration/) | Die maximale Anzahl von Iterationen zur Auflösung eines zirkulären Verweises. |
| [GetMaxChange](./getmaxchange/) | Die maximale Änderung zur Auflösung eines zirkulären Verweises. |
| [SetMaxChange](./setmaxchange/) | Die maximale Änderung zur Auflösung eines zirkulären Verweises. |
| [GetPrecisionAsDisplayed](./getprecisionasdisplayed/) | Gibt an, ob die Präzision des berechneten Ergebnisses so festgelegt wird, wie sie bei der Berechnung von Formeln angezeigt wird. |
| [SetPrecisionAsDisplayed](./setprecisionasdisplayed/) | Gibt an, ob die Präzision des berechneten Ergebnisses so festgelegt wird, wie sie bei der Berechnung von Formeln angezeigt wird. |
| [GetEnableCalculationChain](./getenablecalculationchain/) | Gibt an, ob die Berechnungskette für Formeln aktiviert werden soll. Standard ist false. |
| [SetEnableCalculationChain](./setenablecalculationchain/) | Gibt an, ob die Berechnungskette für Formeln aktiviert werden soll. Standard ist false. |
| [GetPreservePaddingSpaces](./getpreservepaddingspaces/) | Gibt an, ob Leerzeichen und Zeilenumbrüche, die zwischen Formeltoken eingefügt sind, beim Abrufen und Setzen von Formeln erhalten bleiben sollen. Standardwert ist false. |
| [SetPreservePaddingSpaces](./setpreservepaddingspaces/) | Gibt an, ob Leerzeichen und Zeilenumbrüche, die zwischen Formeltoken eingefügt sind, beim Abrufen und Setzen von Formeln erhalten bleiben sollen. Standardwert ist false. |
