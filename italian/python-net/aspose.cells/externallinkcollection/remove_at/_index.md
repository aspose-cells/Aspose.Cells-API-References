---
title: metodo remove_at
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 40
url: /it/python-net/aspose.cells/externallinkcollection/remove_at/
is_root: false
---
##  remove_at(index) {#int}
Rimuove il collegamento esterno specificato dalla cartella di lavoro.



```python
def remove_at(self, index):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| index | int | l'indice del collegamento esterno da rimuovere.|
###  Osservazioni

Quando si rimuove il collegamento esterno, verranno rimosse anche tutte le formule che vi fanno riferimento perché
i riferimenti diventano invalidi.

##  remove_at(index, update_references_as_local) {#int-bool}
Rimuove il collegamento esterno specificato dalla cartella di lavoro.



```python
def remove_at(self, index, update_references_as_local):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| index | int | l'indice del collegamento esterno da rimuovere.|
| update_references_as_local | bool | Se aggiornare tutti i riferimenti di un determinato collegamento esterno al riferimento della cartella di lavoro corrente stessa.|
###  Osservazioni

Se è necessario aggiornare i riferimenti, i riferimenti ai collegamenti esterni nelle formule verranno modificati nella cartella di lavoro corrente.
Ad esempio, il collegamento esterno da rimuovere è "externalsource.xlam" e definisce una funzione personalizzata "customfunction()",
la formula originale di una cella è "='externalsource.xlam'!customfunction()",
dopo aver rimosso la formula diventerà "=customfunction()".
Se il riferimento non è tenuto ad essere aggiornato, tutte le formule con riferimento a questo collegamento esterno
verrà rimosso anche perché quei riferimenti diventano non validi.


###  Guarda anche
* modulo [aspose.cells](../../)
* classe [ExternalLinkCollection](/cells/it/python-net/aspose.cells/externallinkcollection)
