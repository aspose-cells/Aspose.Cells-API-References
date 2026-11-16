---
title: "AbstractCalculationEngine Klasse"
linktitle: "AbstractCalculationEngine"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "AbstractCalculationEngine Klasse. Kapselt das Objekt, das abstractcalculationengine in Go repräsentiert."
type: docs
weight: 200
url: /de/go-cpp/abstractcalculationengine/
---

## AbstractCalculationEngine class

Stellt die benutzerdefinierte Berechnungsengine des Benutzers dar, um die Standard‑Berechnungsengine von Aspose.Cells zu erweitern.

```go

type AbstractCalculationEngine struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [SkipCalculation](./skipcalculation/) | Überspringt die Berechnung der gesamten Formel, die die derzeit ausgewertete Funktion referenziert. |
| [IsParamLiteralRequired](./isparamliteralrequired/) | Gibt an, ob diese Engine den wörtlichen Text des Parameters während einer Berechnung benötigt. Standardwert ist false. |
| [IsParamArrayModeRequired](./isparamarraymoderequired/) | Gibt an, ob diese Engine den Parameter im Array‑Modus berechnen muss. Standardwert ist false. Wenn CalculationData.GetParamValueInArrayMode(int, int, int) beim Berechnen von benutzerdefinierten Funktionen erforderlich ist und der Benutzer die Definition dafür nicht aktualisiert hat (durch Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition)), muss diese Eigenschaft auf true gesetzt werden. |
| [GetProcessBuiltInFunctions](./getprocessbuiltinfunctions/) | Ob integrierte Funktionen, die vom integrierten Engine unterstützt werden, von dieser Implementierung geprüft und verarbeitet werden sollen. Standard ist false. |
| [ForceRecalculate](./forcerecalculate/) | Ob die gegebene Funktion beim Berechnen gemeinsamer Formeln immer neu berechnet werden soll. |
