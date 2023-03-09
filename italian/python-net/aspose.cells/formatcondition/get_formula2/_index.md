---
title: metodo get_formula2
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 30
url: /it/python-net/aspose.cells/formatcondition/get_formula2/
is_root: false
---
##  get_formula2(is_r1c1, is_local) {#bool-bool}
Ottiene il valore o l'espressione associati a questa condizione di formato.


###  ritorna

Il valore o l'espressione associata a questa condizione di formato.


```python
def get_formula2(self, is_r1c1, is_local):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| is_r1c1 | bool | Se la formula deve essere formattata come R1C1.|
| is_local | bool | Se la formula deve essere formattata in base alle impostazioni locali.|


##  get_formula2(row, column) {#int-int}
Ottiene la formula della formattazione condizionale della cella.


###  ritorna

La formula.


```python
def get_formula2(self, row, column):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| row | int | L'indice di riga.|
| column | int | L'indice di colonna.|


##  get_formula2(is_r1c1, is_local, row, column) {#bool-bool-int-int}
Ottiene il valore o l'espressione della formattazione condizionale della cella.


###  ritorna

Il valore o l'espressione associata alla formattazione condizionale della cella.


```python
def get_formula2(self, is_r1c1, is_local, row, column):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| is_r1c1 | bool | Se la formula deve essere formattata come R1C1.|
| is_local | bool | Se la formula deve essere formattata in base alle impostazioni locali.|
| row | int | L'indice di riga.|
| column | int | L'indice di colonna.|
###  Osservazioni

La cella specificata deve essere contenuta da questa formattazione condizionale, altrimenti verrà restituito null.


###  Guarda anche

* modulo [aspose.cells](../../)
* classe [FormatCondition](/cells/it/python-net/aspose.cells/formatcondition)
