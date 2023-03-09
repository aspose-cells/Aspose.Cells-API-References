---
title: metodo index_of
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 40
url: /it/python-net/aspose.cells.properties/builtindocumentpropertycollection/index_of/
is_root: false
---
##  index_of(name) {#str}
Ottiene l'indice di una proprietà in base al nome.


###  ritorna

L'indice a base zero. Valore negativo se non trovato.


```python
def index_of(self, name):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| name | str | Il nome senza distinzione tra maiuscole e minuscole della proprietà.|


##  index_of(item, index) {#DocumentProperty-int}
Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dall'indice specificato all'ultimo elemento.


###  ritorna

L'indice in base zero della prima occorrenza di value all'interno dell'intervallo di elementi nell'elenco di matrici che si estende da startIndex all'ultimo elemento, se trovato; altrimenti, -1.


```python
def index_of(self, item, index):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| item | [DocumentProperty](/cells/it/python-net/aspose.cells.properties/documentproperty) | L'oggetto da individuare nell'elenco dell'array. Il valore può essere nullo.|
| index | int | L'indice iniziale in base zero della ricerca. 0 (zero) è valido in una lista vuota.|


##  index_of(item, index, count) {#DocumentProperty-int-int}
Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che inizia dall'indice specificato e contiene il numero specificato di elementi.


###  ritorna

L'indice in base zero della prima occorrenza di value all'interno dell'intervallo di elementi nell'elenco di matrici che inizia da startIndex e contiene il numero count di elementi, se trovato; altrimenti, -1.


```python
def index_of(self, item, index, count):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| item | [DocumentProperty](/cells/it/python-net/aspose.cells.properties/documentproperty) | L'oggetto da individuare nell'elenco dell'array. Il valore può essere nullo.|
| index | int | L'indice iniziale in base zero della ricerca. 0 (zero) è valido in una lista vuota.|
| count | int | Il numero di elementi nella sezione da cercare.|



###  Guarda anche
* modulo [aspose.cells.properties](../../)
* classe [BuiltInDocumentPropertyCollection](/cells/it/python-net/aspose.cells.properties/builtindocumentpropertycollection)
