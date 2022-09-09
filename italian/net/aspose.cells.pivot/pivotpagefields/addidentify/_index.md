---
title: AddIdentify
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Imposta letichetta dellelemento in ogni campo della pagina da utilizzare per identificare lintervallo di dati. Il pageItemIndex.Length deve essere uguale a PageFieldCount quindi aggiungi prima il campo della pagina.
type: docs
weight: 30
url: /it/net/aspose.cells.pivot/pivotpagefields/addidentify/
---
## PivotPageFields.AddIdentify method

Imposta l'etichetta dell'elemento in ogni campo della pagina da utilizzare per identificare l'intervallo di dati. Il pageItemIndex.Length deve essere uguale a PageFieldCount, quindi aggiungi prima il campo della pagina.

```csharp
public void AddIdentify(int rangeIndex, int[] pageItemIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rangeIndex | Int32 | L'indice dell'intervallo di dati di consolidamento. |
| pageItemIndex | Int32[] | L'indice dell'elemento della pagina nel campo di ogni pagina. pageItemIndex[2] = 1 indica il secondo elemento nel terzo campo da utilizzare per identificare questo intervallo. pageItemIndex[1] = -1 significa nessun elemento nel secondo campo da utilizzare per identificare questo intervallo e MS creerà automaticamente un elemento "vuoto" nel secondo campo per identificare questo intervallo. |

### Guarda anche

* class [PivotPageFields](../../pivotpagefields)
* spazio dei nomi [Aspose.Cells.Pivot](../../pivotpagefields)
* assemblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->