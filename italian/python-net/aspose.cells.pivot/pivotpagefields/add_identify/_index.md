---
title: metodo add_identify
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 20
url: /it/python-net/aspose.cells.pivot/pivotpagefields/add_identify/
is_root: false
---
##  add_identify(range_index, page_item_index) {#int-list}
Imposta l'etichetta dell'elemento in ogni campo della pagina da utilizzare per identificare l'intervallo di dati.
PageItemIndex.Length deve essere uguale a PageFieldCount, quindi aggiungi prima il campo della pagina.



```python
def add_identify(self, range_index, page_item_index):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| range_index | int | L'indice dell'intervallo di dati di consolidamento.|
| page_item_index | list | L'indice dell'elemento della pagina in ogni campo della pagina.<br/>pageItemIndex[2] = 1 indica il secondo elemento nel terzo campo da utilizzare per identificare questo intervallo.<br/> pageItemIndex[1] = -1 indica nessun elemento nel secondo campo da utilizzare per identificare questo intervallo<br/> e MS creerà automaticamente un elemento "vuoto" nel secondo campo per identificare questo intervallo.|



###  Guarda anche
* modulo [aspose.cells.pivot](../../)
* classe [PivotPageFields](/cells/it/python-net/aspose.cells.pivot/pivotpagefields)
