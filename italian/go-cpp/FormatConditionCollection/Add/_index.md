---
title: "Metodo Add"
linktitle: "Aggiungi"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Metodo Add. Incapsula la funzione che rappresenta add in Go."
type: docs
weight: 200
url: /it/go-cpp/formatconditioncollection/add/
---

## Add function

Aggiunge una condizione di formattazione e l'intervallo di celle interessato a FormatConditionsThe FormatConditions può contenere fino a tre conditional formats.Riferimenti ad altri fogli non sono consentiti nelle formule della conditional formatting.

```go

func (instance *FormatConditionCollection) Add(cellarea *CellArea, type_ FormatConditionType, operatortype OperatorType, formula1 string, formula2 string)  ([]int32,  error) 

```

## Osservazioni


## Vedi anche

* Class [FormatConditionCollection](../)
* Library [Aspose.Cells for Go](../../)
