---
title: metodo get_list_value
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 70
url: /it/python-net/aspose.cells/validation/get_list_value/
is_root: false
---
##  get_list_value(row, column) {#int-int}
Ottieni il valore per l'elenco della convalida per la cella specificata.


###  ritorna

Il valore per produrre l'elenco di questa convalida per la cella specificata.
Se l'elenco fa riferimento a un intervallo, il valore restituito sarà un oggetto [ReferredArea](/cells/it/python-net/aspose.cells/referredarea);
In caso contrario, il valore restituito può essere null, oggetto[] o oggetto semplice.


```python
def get_list_value(self, row, column):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| row | int | L'indice di riga.|
| column | int | L'indice di colonna.|
###  Osservazioni

Solo per la convalida il cui tipo è Elenco ed è stato applicato a una determinata cella,
in caso contrario verrà restituito null.


###  Guarda anche
* modulo [aspose.cells](../../)
* classe [ReferredArea](/cells/it/python-net/aspose.cells/referredarea)
* classe [Validation](/cells/it/python-net/aspose.cells/validation)
