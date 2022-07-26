---
title: DataSorter
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Descrizione riepilogativa per DataSorter.
type: docs
weight: 1300
url: /it/net/aspose.cells/datasorter/
---
## DataSorter class

Descrizione riepilogativa per DataSorter.

```csharp
public class DataSorter
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CaseSensitive](../../aspose.cells/datasorter/casesensitive) { get; set; } | Ottiene e imposta la distinzione tra maiuscole e minuscole durante il confronto di string. |
| [HasHeaders](../../aspose.cells/datasorter/hasheaders) { get; set; } | Indica se l'intervallo ha intestazioni. |
| [Key1](../../aspose.cells/datasorter/key1) { get; set; } | Rappresenta il primo indice di colonna ordinato (posizione assoluta, colonna A è 0, B è 1, ...). |
| [Key2](../../aspose.cells/datasorter/key2) { get; set; } | Rappresenta il secondo indice di colonna ordinato (posizione assoluta, colonna A è 0, B è 1, ...). |
| [Key3](../../aspose.cells/datasorter/key3) { get; set; } | Rappresenta il terzo indice di colonna ordinato (posizione assoluta, colonna A è 0, B è 1, ...). |
| [Keys](../../aspose.cells/datasorter/keys) { get; } | Ottiene l'elenco delle chiavi dell'ordinatore di dati. |
| [Order1](../../aspose.cells/datasorter/order1) { get; set; } | Rappresenta l'ordinamento della prima chiave. |
| [Order2](../../aspose.cells/datasorter/order2) { get; set; } | Rappresenta l'ordinamento della seconda chiave. |
| [Order3](../../aspose.cells/datasorter/order3) { get; set; } | Rappresenta l'ordinamento della terza chiave. |
| [SortAsNumber](../../aspose.cells/datasorter/sortasnumber) { get; set; } | Indica se ordinare qualcosa che assomiglia a un numero. |
| [SortLeftToRight](../../aspose.cells/datasorter/sortlefttoright) { get; set; } | True significa che l'orientamento dell'ordinamento è da sinistra a destra. False significa che l'orientamento dell'ordinamento è dall'alto verso il basso. Il valore predefinito è false. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey_1)(int, SortOrder) | Aggiunge l'indice di colonna ordinato e l'ordinamento. |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey_2)(int, SortOrder, string) | Aggiunge l'indice di colonna ordinato e l'ordinamento con un elenco di ordinamento personalizzato. |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey_3)(int, SortOrder, string[]) | Aggiunge l'indice di colonna ordinato e l'ordinamento con un elenco di ordinamento personalizzato. |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey)(int, SortOnType, SortOrder, object) | Aggiunge l'indice di colonna ordinato e l'ordinamento con un elenco di ordinamento personalizzato. |
| [Clear](../../aspose.cells/datasorter/clear)() | Cancella tutte le impostazioni. |
| [Sort](../../aspose.cells/datasorter/sort#sort)() | Ordina i dati nell'intervallo. |
| [Sort](../../aspose.cells/datasorter/sort#sort_1)(Cells, CellArea) | Ordina i dati dell'area. |
| [Sort](../../aspose.cells/datasorter/sort#sort_2)(Cells, int, int, int, int) | Ordina i dati dell'area. |

### Esempi

```csharp

[C#]

//Crea un'istanza di un nuovo oggetto cartella di lavoro.
Workbook workbook = new Workbook("Book1.xls");
//Ottieni l'oggetto datasorter della cartella di lavoro.
DataSorter sorter = workbook.DataSorter;
//Imposta il primo ordine per l'oggetto datasorter.
sorter.Order1 = Aspose.Cells.SortOrder.Descending;
//Definisci la prima chiave.
sorter.Key1 = 0;
//Imposta il secondo ordine per l'oggetto datasorter.
sorter.Order2 = Aspose.Cells.SortOrder.Ascending;
//Definisci la seconda chiave.
sorter.Key2 = 1;
//Crea un'area di celle (intervallo).
CellArea ca = new CellArea();
//Specifica l'indice della riga iniziale.
ca.StartRow = 0;
//Specifica l'indice della colonna iniziale.
ca.StartColumn = 0;
//Specifica l'ultimo indice di riga.
ca.EndRow = 13;
//Specifica l'ultimo indice di colonna.
ca.EndColumn = 1;
//Ordina i dati nell'intervallo di dati specificato (A1:B14)
sorter.Sort(workbook.Worksheets[0].Cells, ca);
//Salva il file excel.
workbook.Save("outBook.xls");

[Visual Basic]

'Crea un'istanza di un nuovo oggetto cartella di lavoro.
Dim workbook As Workbook = New Workbook("Book1.xls")
'Ottieni l'oggetto datasorter della cartella di lavoro.
Dim sorter As DataSorter = workbook.DataSorter
'Imposta il primo ordine per l'oggetto datasorter
sorter.Order1 = Aspose.Cells.SortOrder.Descending
'Definisci la prima chiave.
sorter.Key1 = 0
'Imposta il secondo ordine per l'oggetto datasorter.
sorter.Order2 = Aspose.Cells.SortOrder.Ascending
'Definisci la seconda chiave.
sorter.Key2 = 1
'Crea un'area di celle (intervallo).
Dim ca As CellArea = New CellArea
'Specificare l'indice della riga iniziale.
ca.StartRow = 0
'Specificare l'indice della colonna iniziale.
ca.StartColumn = 0
'Specificare l'ultimo indice di riga.
ca.EndRow = 13
'Specificare l'ultimo indice di colonna.
ca.EndColumn = 1
'Ordina i dati nell'intervallo di dati specificato (A1:B14)
sorter.Sort(workbook.Worksheets(0).Cells, ca)
'Salva il file excel.
workbook.Save("outBook.xls")

```

### Guarda anche

* spazio dei nomi [Aspose.Cells](../../aspose.cells)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
