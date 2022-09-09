---
title: GetStyleInPool
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Ottiene lo stile nel pool di stili. Tutti gli stili nella cartella di lavoro verranno raccolti in un pool. Nelle celle è presente solo un semplice indice di riferimento.
type: docs
weight: 450
url: /it/net/aspose.cells/workbook/getstyleinpool/
---
## Workbook.GetStyleInPool method

Ottiene lo stile nel pool di stili. Tutti gli stili nella cartella di lavoro verranno raccolti in un pool. Nelle celle è presente solo un semplice indice di riferimento.

```csharp
public Style GetStyleInPool(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | Int32 | L'indice. |

### Valore di ritorno

Lo stile nel pool corrisponde a un dato indice, può essere null.

### Osservazioni

Se lo stile restituito viene modificato, lo stile di tutte le celle (che si riferisce a questo stile) verrà modificato.

### Guarda anche

* class [Style](../../style)
* class [Workbook](../../workbook)
* spazio dei nomi [Aspose.Cells](../../workbook)
* assemblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->