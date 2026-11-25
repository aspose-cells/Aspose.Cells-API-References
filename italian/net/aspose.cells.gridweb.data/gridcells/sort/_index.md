---
title: "GridCells.Sort"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GridCells. Ordina i dati in ordine ascendente/descendente dall'alto verso il basso in un intervallo di un foglio di lavoro per indice di colonna specificato. Ordina i dati in ordine ascendente/descendente da sinistra a destra in un intervallo di un foglio di lavoro per indice di riga specificato"
type: docs
url: /it/net/aspose.cells.gridweb.data/gridcells/sort/
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
 GridWeb GridWeb1 = new GridWeb();
 GridWeb1.WorkSheets[0].Cells.Sort(1,0,25,6,3,true,true,false);

 [VB]

 GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3,true,true,false)

```

### Vedi anche

* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) {#sort_1}

Ordina i dati in modo ascendente/decendente dall'alto verso il basso in un intervallo di un Worksheet secondo l'indice di colonna specificato. Ordina i dati in modo ascendente/decendente da sinistra a destra in un intervallo di un Worksheet secondo l'indice di riga specificato.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes, 
    SortByOrder[] orders, SortOrientation orientation, bool isCaseSensitive)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | Il numero di riga della prima cella da ordinare. |
| startColumn | Int32 | Il numero di colonna della prima cella da ordinare. |
| righe | Int32 | Numero di righe da importare. |
| colonne | Int32 | Numero di colonne da importare. |
| indici | Int32[] | L'array di indici di colonna che specifica la colonna di ordinamento. Se l'Orientamento è dall'alto verso il basso, rappresenta l'indice di colonna che specifica la colonna di ordinamento. Se l'Orientamento è da sinistra a destra, rappresenta l'indice di riga che specifica la riga di ordinamento. |
| ordini | SortByOrder[] | l'array dell'ordine di ordinamento. |
| orientamento | SortOrientation | orientamento di ordinamento |
| isCaseSensitive | Booleano | se l'ordinamento è sensibile al maiuscolo/minuscolo. |

### Esempi

```csharp

 [C#]
 GridWeb GridWeb1=new GridWeb();
 int[] ids={0,1};
 SortByOrder[] sorder={SortByOrder.Ascending,SortByOrder.Descending};
 GridWeb1.WorkSheets[0].Cells.Sort(1,0,25,6,ids,sorder,SortOrientation.SortTopToBottom,false);

 [VB]

 GridWeb1.WorkSheets(0).Cells.Sort(1,0,25,6,ids,sorder,SortOrientation.SortTopToBottom,false)

```

### Vedi anche

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


