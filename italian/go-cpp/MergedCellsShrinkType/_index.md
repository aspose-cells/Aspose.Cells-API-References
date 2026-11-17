---
title: "MergedCellsShrinkType Enum"
linktitle: "MergedCellsShrinkType"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "MergedCellsShrinkType enum. Incapsula l'oggetto che rappresenta mergedcellsshrinktype in Go."
type: docs
weight: 200
url: /it/go-cpp/mergedcellsshrinktype/
---

## MergedCellsShrinkType Enum

Rappresenta la strategia per ridurre le celle unite per operazioni come l'eliminazione di righe/colonne vuote.

```go

type MergedCellsShrinkType int32


```

## Campi

| Campo | Descrizione |
| --- | --- |
| [None](./none/) | Lascia le celle unite così come sono, senza alcuna modifica. |
| [ShrinkToFit](./shrinktofit/) | Riduce l'area unita se necessario, rimuovendo le righe dalla parte inferiore o le colonne da quella destra, garantendo che tutto il contenuto rimanga visibile. |
| [KeepHeaderOnly](./keepheaderonly/) | Mantiene solo le righe/colonne di intestazione dell'area unita quando la cella in alto a sinistra dell'area unita non è vuota. |
