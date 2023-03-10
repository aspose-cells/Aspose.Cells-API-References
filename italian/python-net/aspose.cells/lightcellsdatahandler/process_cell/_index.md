---
title: metodo process_cell
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 20
url: /it/python-net/aspose.cells/lightcellsdatahandler/process_cell/
is_root: false
---
##  process_cell(cell) {#Cell}
Inizia a elaborare una cella.


###  ritorna

se questa cella deve essere mantenuta nel modello di celle del foglio corrente.
Normalmente dovrebbe essere falso in modo che tutte le celle non vengano mantenute in memoria dopo essere state elaborate e quindi la memoria venga salvata.
Per alcuni scopi speciali, ad esempio l'utente deve accedere ad alcune celle in un secondo momento dopo che l'intera cartella di lavoro è stata elaborata,
l'utente può fare in modo che questo metodo restituisca true per mantenere quelle celle speciali nel modello Cells e accedervi successivamente tramite API come Cells[riga, colonna].
Tuttavia, mantenere i dati delle celle nel modello Cells richiederà più memoria e se tutte le celle vengono conservate, leggere il file modello
in modalità LightCells diventerà lo stesso leggendolo in modo normale.


```python
def process_cell(self, cell):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| cell | [Cell](/cells/it/python-net/aspose.cells/cell) | Cell oggetto attualmente in fase di elaborazione|
###  Osservazioni

Verrà chiamato dopo che i dati di una cella sono stati letti.


###  Guarda anche

* modulo [aspose.cells](../../)
* classe [LightCellsDataHandler](/cells/it/python-net/aspose.cells/lightcellsdatahandler)
