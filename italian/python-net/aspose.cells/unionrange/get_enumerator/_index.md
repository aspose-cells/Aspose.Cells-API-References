---
title: metodo get_enumerator
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 40
url: /it/python-net/aspose.cells/unionrange/get_enumerator/
is_root: false
---
##  get_enumerator() {#}
Ottiene l'enumeratore per le celle in questo Range.


###  ritorna

L'enumeratore di celle


```python
def get_enumerator(self):
    ...
```


###  Osservazioni

Quando si attraversano gli elementi dall'enumeratore restituito, la raccolta di celle
non deve essere modificato (come le operazioni che provocheranno la creazione di un'istanza del nuovo Cell/Row o l'eliminazione di Cell/Row esistente).
In caso contrario, l'enumeratore potrebbe non essere in grado di attraversare correttamente tutte le celle (alcuni elementi potrebbero essere attraversati ripetutamente o ignorati).


###  Guarda anche
* modulo [aspose.cells](../../)
* classe [UnionRange](/cells/it/python-net/aspose.cells/unionrange)
