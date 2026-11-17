---
title: "IsParamArrayModeRequired Metodo"
linktitle: "IsParamArrayModeRequired"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "IsParamArrayModeRequired metodo. Incapsula la funzione che rappresenta isparamarraymoderequired in Go."
type: docs
weight: 200
url: /it/go-cpp/abstractcalculationengine/isparamarraymoderequired/
---

## IsParamArrayModeRequired function

Indica se questo motore necessita che il parametro sia calcolato in modalità array. Il valore predefinito è false. Se CalculationData.GetParamValueInArrayMode(int, int, int) è richiesto durante il calcolo di customfunctions e l'utente non ha aggiornato la definizione per esse (tramite Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition)), questa proprietà deve essere impostata su true.

```go

func (instance *AbstractCalculationEngine) IsParamArrayModeRequired()  (bool,  error) 

```

## Osservazioni


## Vedi anche

* Class [AbstractCalculationEngine](../)
* Library [Aspose.Cells for Go](../../)
