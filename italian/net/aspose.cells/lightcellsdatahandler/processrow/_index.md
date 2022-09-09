---
title: ProcessRow
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Inizia a elaborare una riga.
type: docs
weight: 20
url: /it/net/aspose.cells/lightcellsdatahandler/processrow/
---
## LightCellsDataHandler.ProcessRow method

Inizia a elaborare una riga.

```csharp
public bool ProcessRow(Row row)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| row | Row | Oggetto riga attualmente in elaborazione. |

### Valore di ritorno

se le celle di questa riga devono essere elaborate. false per ignorare tutte le celle in questa riga.

### Osservazioni

Verrà chiamato dopo le proprietà della riga come altezza, stile, ...ecc. sono stati letti. Tuttavia, le celle in questa riga non sono state ancora lette.

### Guarda anche

* class [Row](../../row)
* interface [LightCellsDataHandler](../../lightcellsdatahandler)
* spazio dei nomi [Aspose.Cells](../../lightcellsdatahandler)
* assemblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->