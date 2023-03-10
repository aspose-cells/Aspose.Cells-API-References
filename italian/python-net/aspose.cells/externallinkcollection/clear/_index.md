---
title: metodo clear
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 30
url: /it/python-net/aspose.cells/externallinkcollection/clear/
is_root: false
---
##  clear() {#}
Rimuove tutti i link esterni.



```python
def clear(self):
    ...
```


###  Osservazioni

Quando si rimuovono i collegamenti esterni, verranno rimosse anche tutte le formule che vi fanno riferimento perché
i riferimenti diventano invalidi.

##  clear(update_references_as_local) {#bool}
Rimuove tutti i link esterni.



```python
def clear(self, update_references_as_local):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| update_references_as_local | bool | Se aggiornare tutti i riferimenti dei collegamenti esterni come riferimenti della cartella di lavoro corrente stessa.|
###  Osservazioni

Se è necessario aggiornare i riferimenti, i riferimenti ai collegamenti esterni nelle formule verranno modificati nella cartella di lavoro corrente.
Ad esempio, la formula originale di una cella è "='externalsource.xlam'!customfunction()",
dopo aver rimosso i link esterni, la formula diventerà "=customfunction()".
Se i riferimenti non devono essere aggiornati, tutte le formule con riferimenti a collegamenti esterni
verrà rimosso anche perché quei riferimenti diventano non validi.


###  Guarda anche
* modulo [aspose.cells](../../)
* classe [ExternalLinkCollection](/cells/it/python-net/aspose.cells/externallinkcollection)
