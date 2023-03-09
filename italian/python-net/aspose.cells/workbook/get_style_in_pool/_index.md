---
title: metodo get_style_in_pool
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 190
url: /it/python-net/aspose.cells/workbook/get_style_in_pool/
is_root: false
---
##  get_style_in_pool(index) {#int}
Ottiene lo stile nel pool di stili.
Tutti gli stili nella cartella di lavoro verranno raccolti in un pool.
C'è solo un semplice indice di riferimento nelle celle.


###  ritorna

Lo stile nel pool corrisponde a un dato indice, può essere nullo.


```python
def get_style_in_pool(self, index):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| index | int | L'indice.|
###  Osservazioni

Se lo stile restituito viene modificato, lo stile di tutte le celle (che fa riferimento a questo stile) verrà modificato.


###  Guarda anche

* modulo [aspose.cells](../../)
* classe [Workbook](/cells/it/python-net/aspose.cells/workbook)
