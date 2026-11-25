---
title: "WebCells.Sort"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WebCells. Ordina i dati in modo ascendente dall'alto verso il basso in un intervallo di un WebWorksheet per indice di colonna specificato"
type: docs
url: /it/net/aspose.cells.gridweb.data/webcells/sort/
---
## Sort(int, int, int, int, int) {#sort}

Ordina i dati in ordine ascendente dall'alto verso il basso in un intervallo di un WebWorksheet per indice di colonna specificato.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | Il numero di riga della prima cella da ordinare. |
| startColumn | Int32 | Il numero di colonna della prima cella da ordinare. |
| righe | Int32 | Numero di righe da importare. |
| colonne | Int32 | Numero di colonne da importare. |
| indice | Int32 | L'indice di colonna che specifica la colonna di ordinamento. |

### Esempi

```csharp

[C#]

GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,3);

[VB]

GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3)

```

### Vedi anche

* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int, SortByOrder, SortOrientation, bool) {#sort_1}

Ordina i dati in ordine ascendente dall'alto verso il basso in un intervallo di un WebWorksheet per indice di colonna specificato.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index, 
    SortByOrder sortOrder, SortOrientation sortOrientation, bool isCaseSensitive)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | Il numero di riga della prima cella da ordinare. |
| startColumn | Int32 | Il numero di colonna della prima cella da ordinare. |
| righe | Int32 | Numero di righe da importare. |
| colonne | Int32 | Numero di colonne da importare. |
| indice | Int32 | L'indice di colonna (o riga) che specifica la colonna (o riga) di ordinamento. Se l'orientamento dell'ordinamento è dall'alto verso il basso, l'indice rappresenta l'indice di colonna. Se l'orientamento è da sinistra a destra, l'indice rappresenta l'indice di riga. |
| ordine | SortByOrder | L'ordine di ordinamento: Ascendente o Discendente |
| orientamento | SortOrientation | L'orientamento dell'ordinamento: dall'alto verso il basso o da sinistra a destra. |
| isCaseSensitive | Booleano | Indica se i dati da ordinare sono sensibili al maiuscolo/minuscolo quando i dati sono stringa. |

### Esempi

```csharp

[C#]

GridWeb1.WebWorksheets[0].Cells.Sort(0,1,4,14,3,SortOrder.Ascending,SortOrientation.SortLeftToRight,true)

[VB]

GridWeb1.WebWorksheets(0).Cells.Sort(0,1,4,14,3,SortOrder.Ascending,SortOrientation.SortLeftToRight,True)

```

### Vedi anche

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[]) {#sort_2}

Ordina i dati in ordine ascendente dall'alto verso il basso in un intervallo di un WebWorksheet per alcuni campi specificati da un array di indici di colonna.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | Il numero di riga della prima cella da ordinare. |
| startColumn | Int32 | Il numero di colonna della prima cella da ordinare. |
| righe | Int32 | Numero di righe da importare. |
| colonne | Int32 | Numero di colonne da importare. |
| indici | Int32[] | L'array di indici di colonna che specifica i dati da ordinare. |

### Esempi

```csharp

[C#]

int[] indexes = new int[3];
indexes[0] = 0;
indexes[1] = 2;
indexes[2] = 3;
GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,indexes);

[VB]

Dim indexes() As Integer =  New Integer(3) {} 
indexes(0) = 0
indexes(1) = 2
indexes(2) = 3
GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,indexes)

```

### Vedi anche

* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) {#sort_3}

Ordina i dati in ordine ascendente in un intervallo di un WebWorksheet per alcuni campi specificati da un array di indici.

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
| indici | Int32[] | L'indice di colonna (o riga) che specifica la colonna (o riga) di ordinamento. Se l'orientamento dell'ordinamento è dall'alto verso il basso, l'indice rappresenta l'indice di colonna. Se l'orientamento è da sinistra a destra, l'indice rappresenta l'indice di riga. |
| ordini | SortByOrder[] | L'ordine di ordinamento: Ascendente o Discendente |
| orientamento | SortOrientation | L'orientamento dell'ordinamento: dall'alto verso il basso o da sinistra a destra. |
| isCaseSensitive | Booleano | Indica se l'ordinamento è sensibile al maiuscolo/minuscolo. |

### Osservazioni

Se utilizzi questo metodo per ordinare un blocco di dati, assicurati che la lunghezza del parametro indici sia uguale alla lunghezza del parametro ordini.

### Esempi

```csharp

```

[C#] int[] indexes = new int[3]; indexes[0] = 0; indexes[1] = 1; indexes[2] = 3; SortOrder[] orders = new SortOrder[3]; orders[0] = SortOrder.Ascending; orders[1] = SortOrder.Descending; orders[2] = SortOrder.Descending; GridWeb1.WebWorksheets[0].Cells.Sort(0,1,4,14,indexes,orders,SortOrientation.SortLeftToRight,false); [VB] Dim indexes() As Integer = New Integer(3) {} indexes(0) = 0 indexes(1) = 1 indexes(2) = 3 Dim orders() As SortOrder = New SortOrder(3) {} orders(0) = SortOrder.Ascending orders(1) = SortOrder.Descending orders(2) = SortOrder.Descending GridWeb1.WebWorksheets(0).Cells.Sort(0,1,4,14,indexes,orders,SortOrientation.SortLeftToRight,False)

### Vedi anche

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


