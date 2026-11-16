---
title: "CalculationOptions Klasse"
linktitle: "CalculationOptions"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "CalculationOptions-Klasse. Kapselt das Objekt, das calculationoptions in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/calculationoptions/
---

## CalculationOptions class

Stellt Optionen für die Berechnung dar.

```go

type CalculationOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewCalculationOptions](./newcalculationoptions/) | Standardkonstruktor. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetIgnoreError](./getignoreerror/) | Gibt an, ob beim Berechnen von Formeln auftretende Fehler ignoriert werden sollen. Der Fehler kann eine nicht unterstützte Funktion, externe Links usw. sein. Der Standardwert ist true. |
| [SetIgnoreError](./setignoreerror/) | Gibt an, ob beim Berechnen von Formeln auftretende Fehler ignoriert werden sollen. Der Fehler kann eine nicht unterstützte Funktion, externe Links usw. sein. Der Standardwert ist true. |
| [GetRecursive](./getrecursive/) | Gibt an, ob abhängige Zellen rekursiv berechnet werden sollen, wenn eine Zelle berechnet wird und von anderen Zellen abhängt. Der Standardwert ist true. |
| [SetRecursive](./setrecursive/) | Gibt an, ob abhängige Zellen rekursiv berechnet werden sollen, wenn eine Zelle berechnet wird und von anderen Zellen abhängt. Der Standardwert ist true. |
| [GetUserSpecifiedRefreshDynamicArrayFormula](./getuserspecifiedrefreshdynamicarrayformula/) | Gibt an, ob der Benutzer das Verhalten des Aktualisierens dynamischer Array-Formeln vor dem Berechnen bestimmter Formeln explizit angegeben hat. |
| [GetRefreshDynamicArrayFormula](./getrefreshdynamicarrayformula/) | Gibt an, ob dynamische Array-Formeln vor dem Berechnen von Formeln aktualisiert werden sollen. |
| [SetRefreshDynamicArrayFormula](./setrefreshdynamicarrayformula/) | Gibt an, ob dynamische Array-Formeln vor dem Berechnen von Formeln aktualisiert werden sollen. |
| [GetCustomEngine](./getcustomengine/) | Die benutzerdefinierte Formelberechnungs-Engine, um die Standardberechnungs-Engine von Aspose.Cells zu erweitern. |
| [SetCustomEngine](./setcustomengine/) | Die benutzerdefinierte Formelberechnungs-Engine, um die Standardberechnungs-Engine von Aspose.Cells zu erweitern. |
| [GetCalcStackSize](./getcalcstacksize/) | Die Stapelgröße für die rekursive Berechnung von Zellen. Standardwert ist 200. |
| [SetCalcStackSize](./setcalcstacksize/) | Die Stapelgröße für die rekursive Berechnung von Zellen. Standardwert ist 200. |
| [GetPrecisionStrategy](./getprecisionstrategy/) | Gibt die Strategie für die Verarbeitung der Berechnungsgenauigkeit an. |
| [SetPrecisionStrategy](./setprecisionstrategy/) | Gibt die Strategie für die Verarbeitung der Berechnungsgenauigkeit an. |
| [GetLinkedDataSources](./getlinkeddatasources/) | Gibt die Datenquellen für in Formeln verwendete externe Links an. |
| [SetLinkedDataSources](./setlinkeddatasources/) | Gibt die Datenquellen für in Formeln verwendete externe Links an. |
| [GetCharacterEncoding](./getcharacterencoding/) | Gibt die Kodierung an, die beim Kodieren/Dekodieren von Zeichen während der Berechnung von Formeln verwendet wird. Für Funktionen wie CHAR, CODE hängt das berechnete Ergebnis von den Regionseinstellungen und dem Standard‑Zeichensatz der Umgebung ab. Mit dieser Eigenschaft kann der Benutzer die geeignete Kodierung für diese Funktionen angeben, um das erwartete Ergebnis zu erhalten. |
| [SetCharacterEncoding](./setcharacterencoding/) | Gibt die Kodierung an, die beim Kodieren/Dekodieren von Zeichen während der Berechnung von Formeln verwendet wird. Für Funktionen wie CHAR, CODE hängt das berechnete Ergebnis von den Regionseinstellungen und dem Standard‑Zeichensatz der Umgebung ab. Mit dieser Eigenschaft kann der Benutzer die geeignete Kodierung für diese Funktionen angeben, um das erwartete Ergebnis zu erhalten. |
