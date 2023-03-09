---
title: metodo update_linked_data_source
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 410
url: /it/python-net/aspose.cells/workbook/update_linked_data_source/
is_root: false
---
##  update_linked_data_source(external_workbooks) {#list}
Se questa cartella di lavoro contiene collegamenti esterni ad altre origini dati,
Aspose.Cells tenterà di recuperare i dati più recenti.



```python
def update_linked_data_source(self, external_workbooks):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| external_workbooks | list | Le cartelle di lavoro esterne sono referenziate da questa cartella di lavoro.<br/>Se è nullo, apriremo direttamente i file collegati esterni.<br/> Se non è nullo,<br/>controlleremo prima se il collegamento esterno nell'array;<br/> in caso contrario, apriremo nuovamente i file collegati esterni.|
###  Osservazioni

Se il metodo non viene chiamato prima del calcolo delle formule,
Aspose.Cells utilizzerà le informazioni precedenti (memorizzate nella cache del file);
 Impostare CellsHelper.StartupPath, CellsHelper.AltStartPath, CellsHelper.LibraryPath.
E per favore imposta Workbook.FilePath se questa cartella di lavoro proviene da un flusso,
altrimenti Aspose.Cells a volte non riusciva a ottenere il percorso completo del collegamento esterno.


###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Workbook](/cells/it/python-net/aspose.cells/workbook)
