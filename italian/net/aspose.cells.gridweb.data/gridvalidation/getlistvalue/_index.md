---
title: "GridValidation.GetListValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GridValidation. Ottiene il valore per l'elenco della convalida per la cella specificata."
type: docs
url: /it/net/aspose.cells.gridweb.data/gridvalidation/getlistvalue/
---
## GridValidation.GetListValue method

Ottieni il valore per l'elenco della convalida per la cella specificata.

```csharp
public object GetListValue(int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | L'indice della riga. |
| colonna | Int32 | L'indice della colonna. |

### Valore di ritorno

Il valore per generare l'elenco di questa convalida per la cella specificata. Se l'elenco fa riferimento a un intervallo, il valore restituito sarà un oggetto ReferredArea; altrimenti il valore restituito può essere null, object[] o un semplice oggetto.

### Osservazioni

Solo per le convalide il cui tipo è List e che sono state applicate alla cella indicata; altrimenti verrà restituito null.

### Vedi anche

* class [GridValidation](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


