---
title: metodo get_linked_cell
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 100
url: /it/python-net/aspose.cells.drawing/shape/get_linked_cell/
is_root: false
---
##  get_linked_cell(is_r1c1, is_local) {#bool-bool}
Ottiene l'intervallo collegato al valore del controllo.


###  ritorna

L'intervallo collegato al valore del controllo.


```python
def get_linked_cell(self, is_r1c1, is_local):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| is_r1c1 | bool | Se la formula deve essere formattata come R1C1.|
| is_local | bool | Se la formula deve essere formattata in base alle impostazioni locali.|

###  Esempio

```python

# You may get results like '$A$1'
link = shape.get_linked_cell(False, False)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [Shape](/cells/it/python-net/aspose.cells.drawing/shape)
