---
title: "IsParamArrayModeRequired Methode"
linktitle: "IsParamArrayModeRequired"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "IsParamArrayModeRequired Methode. Kapselt die Funktion, die isparamarraymoderequired in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/abstractcalculationengine/isparamarraymoderequired/
---

## IsParamArrayModeRequired function

Gibt an, ob diese Engine den Parameter im Array‑Modus berechnen muss. Standardwert ist false. Wenn CalculationData.GetParamValueInArrayMode(int, int, int) beim Berechnen von benutzerdefinierten Funktionen erforderlich ist und der Benutzer die Definition dafür nicht aktualisiert hat (durch Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition)), muss diese Eigenschaft auf true gesetzt werden.

```go

func (instance *AbstractCalculationEngine) IsParamArrayModeRequired()  (bool,  error) 

```

## Hinweise


## Siehe auch

* Class [AbstractCalculationEngine](../)
* Library [Aspose.Cells for Go](../../)
