---
title: metodo get_value
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 20
url: /it/python-net/aspose.cells/referredarea/get_value/
is_root: false
---
##  get_value(row_offset, col_offset) {#int-int}
Ottiene il valore della cella con un determinato offset dall'angolo in alto a sinistra di quest'area.


###  ritorna

"#REF!" se quest'area non è valida;
"#N/A" se viene specificato l'offset al di fuori di quest'area;
Altrimenti restituisce il valore della cella in una data posizione.


```python
def get_value(self, row_offset, col_offset):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| row_offset | int | scostamento riga dalla riga iniziale di quest'area|
| col_offset | int |scostamento di colonna dalla riga iniziale di quest'area|


##  get_value(row_offset, col_offset, calculate_formulas) {#int-int-bool}
Ottiene il valore della cella con un determinato offset dall'angolo in alto a sinistra di quest'area.


###  ritorna

"#REF!" se quest'area non è valida;
"#N/A" se viene specificato l'offset al di fuori di quest'area;
Altrimenti restituisce il valore della cella in una data posizione.


```python
def get_value(self, row_offset, col_offset, calculate_formulas):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| row_offset | int | scostamento riga dalla riga iniziale di quest'area|
| col_offset | int |scostamento di colonna dalla riga iniziale di quest'area|
| calculate_formulas | bool | Se lo calcola in modo ricorsivo se il riferimento specificato è una formula|



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [ReferredArea](/cells/it/python-net/aspose.cells/referredarea)
