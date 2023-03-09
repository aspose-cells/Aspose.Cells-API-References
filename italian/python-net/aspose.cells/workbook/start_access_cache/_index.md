---
title: metodo start_access_cache
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 380
url: /it/python-net/aspose.cells/workbook/start_access_cache/
is_root: false
---
##  start_access_cache(opts) {#AccessCacheOptions}
Avvia la sessione che utilizza le cache per accedere ai dati.



```python
def start_access_cache(self, opts):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| opts | [AccessCacheOptions](/cells/it/python-net/aspose.cells/accesscacheoptions) | opzioni di accesso ai dati|
###  Osservazioni

Se la cache dell'accesso ai dati specificato richiede che alcuni modelli di dati nel foglio di lavoro siano "di sola lettura",
quindi i modelli di dati corrispondenti in ogni foglio di lavoro in questa cartella di lavoro verranno presi come "sola lettura"
e l'utente non dovrebbe cambiarne nessuno.


Dopo aver terminato l'accesso ai dati, [Workbook.close_access_cache(opts)](/cells/it/python-net/aspose.cells/workbook/close_access_cache) dovrebbe
essere richiamato con le stesse opzioni per cancellare tutte le cache e ripristinare la normale modalità di accesso.


###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Workbook](/cells/it/python-net/aspose.cells/workbook)
