---
title: "Worksheet.AddCustomFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Aggiunge un filtro personalizzato per l'intervallo di righe specificato dalla riga iniziale alla riga finale"
type: docs
url: /it/net/aspose.cells.griddesktop/worksheet/addcustomfilter/
---
## AddCustomFilter(int, int, object[], GridFilterOperatorType[]) {#addcustomfilter}

Aggiunge un filtro personalizzato per l'intervallo di righe specificato dalla riga iniziale alla riga finale.

```csharp
public void AddCustomFilter(int startrow, int startcolumn, object[] critiras, 
    GridFilterOperatorType[] filterOperatorTypes)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startrow | Int32 | La startrow dell'intervallo del filtro |
| startcolumn | Int32 | La startcolumn dell'intervallo del filtro |
| critiras | Object[] | L'array critira per le colonne, ognuno si applica a ciascuna colonna |
| filterOperatorTypes | GridFilterOperatorType[] | L'array dei tipi di operatore di filtro per le colonne, ognuno si applica a ciascuna colonna |

### Vedi anche

* enum [GridFilterOperatorType](../../../aspose.cells.griddesktop.data/gridfilteroperatortype/)
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## AddCustomFilter(int, string) {#addcustomfilter_1}

Aggiunge un filtro personalizzato per la riga specificata.

```csharp
public void AddCustomFilter(int row, string critira)
```

### Osservazioni

La stringa dei criteri di filtro. Nota che usiamo , e ; come caratteri di separazione, quindi il valore della cella non deve contenere questi caratteri di separazione. Di seguito sono riportati esempi di stringhe di criteri: //column 0 with value 12.3 CELL0 = 12.3 //column 1 with value ABC CELL1 = ABC //column 0 with value 123 or 456 or ABC and column 1 with value ABC CELL0 = 123,456,ABC; CELL1 = ABC

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


