---
title: Subtotal
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Crea i totali parziali per lintervallo.
type: docs
weight: 1310
url: /it/net/aspose.cells/cells/subtotal/
---
## Subtotal(CellArea, int, ConsolidationFunction, int[]) {#subtotal}

Crea i totali parziali per l'intervallo.

```csharp
public void Subtotal(CellArea ca, int groupBy, ConsolidationFunction function, int[] totalList)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ca | CellArea | La gamma |
| groupBy | Int32 | Il campo in base al quale raggruppare, come offset intero in base zero |
| function | ConsolidationFunction | La funzione del totale parziale. |
| totalList | Int32[] | Una matrice di offset di campo in base zero, che indica i campi a cui vengono aggiunti i totali parziali. |

### Guarda anche

* struct [CellArea](../../cellarea)
* enum [ConsolidationFunction](../../consolidationfunction)
* class [Cells](../../cells)
* spazio dei nomi [Aspose.Cells](../../cells)
* assemblea [Aspose.Cells](../../../)

---

## Subtotal(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) {#subtotal_1}

Crea i totali parziali per l'intervallo.

```csharp
public void Subtotal(CellArea ca, int groupBy, ConsolidationFunction function, int[] totalList, 
    bool replace, bool pageBreaks, bool summaryBelowData)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ca | CellArea | La gamma |
| groupBy | Int32 | Il campo in base al quale raggruppare, come offset intero in base zero |
| function | ConsolidationFunction | La funzione del totale parziale. |
| totalList | Int32[] | Una matrice di offset di campo in base zero, che indica i campi a cui vengono aggiunti i totali parziali. |
| replace | Boolean | Indica se sostituire i totali parziali correnti |
| pageBreaks | Boolean | Indica se aggiungere un'interruzione di pagina tra i gruppi |
| summaryBelowData | Boolean | Indica se aggiungere un riepilogo sotto i dati. |

### Guarda anche

* struct [CellArea](../../cellarea)
* enum [ConsolidationFunction](../../consolidationfunction)
* class [Cells](../../cells)
* spazio dei nomi [Aspose.Cells](../../cells)
* assemblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
