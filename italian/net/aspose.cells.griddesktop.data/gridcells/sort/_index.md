---
title: "GridCells.Sort"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GridCells. Ordina i dati in ordine ascendente/descendente dall'alto verso il basso in un intervallo di un foglio di lavoro per indice di colonna specificato. Ordina i dati in ordine ascendente/descendente da sinistra a destra in un intervallo di un foglio di lavoro per indice di riga specificato"
type: docs
url: /it/net/aspose.cells.griddesktop.data/gridcells/sort/
---
## Sort(int, int, int, int, int, bool, bool, bool) {#sort}

Ordina i dati in modo ascendente/decendente dall'alto verso il basso in un intervallo di un Worksheet secondo l'indice di colonna specificato. Ordina i dati in modo ascendente/decendente da sinistra a destra in un intervallo di un Worksheet secondo l'indice di riga specificato.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index, bool isAsending, 
    bool isCaseSensitive, bool islefttoright)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | Il numero di riga della prima cella da ordinare. |
| startColumn | Int32 | Il numero di colonna della prima cella da ordinare. |
| righe | Int32 | Numero di righe da importare. |
| colonne | Int32 | Numero di colonne da importare. |
| indice | Int32 | L'indice di colonna che specifica la colonna di ordinamento. se l'Orientation è dall'alto verso il basso, rappresenta l'indice di colonna che specifica la colonna di ordinamento. se l'Orientation è da sinistra a destra, rappresenta l'indice di riga che specifica la riga di ordinamento. |
| isAsending | Booleano | se l'ordine di ordinamento è ascendente. |
| isCaseSensitive | Booleano | se l'ordinamento è sensibile al maiuscolo/minuscolo. |
| islefttoright | Booleano | se l'orientamento dell'ordinamento è da sinistra a destra |

### Esempi

```csharp

 [C#]

 GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,3,true,true,false);

 [VB]

 GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3,true,true,false)

```

### Vedi anche

* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Sort(int, int, int, int, int[], SortOrder[], SortOrientation, bool) {#sort_1}

Ordina i dati dell'area.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes, 
    SortOrder[] orders, SortOrientation orientation, bool isCaseSensitive)
```

| Parametro | Descrizione |
| --- | --- |
| celle | Le celle contengono l'area dei dati. |
| startRow | La riga iniziale dell'area. |
| startColumn | La colonna iniziale dell'area. |
| righe | il numero totale di righe. |
| colonne | Il numero totale di colonne. |
| indici | L'array di indici di colonna ordinati |
| ordini | L'array di ordini ordinati |
| orientamento | l'orientamento di ordinamento: da sinistra a destra o dall'alto verso il basso. |
| isCaseSensitive | se è sensibile al maiuscolo/minuscolo durante il confronto delle stringhe.. |

### Vedi anche

* enum [SortOrder](../../../aspose.cells.griddesktop/sortorder/)
* enum [SortOrientation](../../../aspose.cells.griddesktop/sortorientation/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


