---
title: classe LoadFilter
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 1010
url: /it/python-net/aspose.cells/loadfilter/
is_root: false
---
##  classe LoadFilter
Rappresenta il filtro che fornisce le opzioni per il caricamento dei dati durante il caricamento della cartella di lavoro dal modello.



Il tipo LoadFilter espone i membri seguenti:

###  Costruttori
| Costruttore| Descrizione|
| :- | :- |
| [LoadFilter()](/cells/it/python-net/aspose.cells/loadfilter/__init__/#) | Costruisce un LoadFilter con opzioni di filtro predefinite LoadDataFilterOptions.All.|
| [LoadFilter(opts)](/cells/it/python-net/aspose.cells/loadfilter/__init__/#LoadDataFilterOptions) | Costruisce un LoadFilter con determinate opzioni di filtro.|


###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [load_data_filter_options](/cells/it/python-net/aspose.cells/loadfilter/load_data_filter_options) | Le opzioni di filtro per indicare quali dati devono essere caricati.|
| [sheets_in_loading_order](/cells/it/python-net/aspose.cells/loadfilter/sheets_in_loading_order) | Specifica i fogli (indici) e l'ordine da caricare.<br/>L'impostazione predefinita è null, che indica di caricare tutti i fogli nell'ordine predefinito nel file modello.<br/> Se non è nullo e l'indice di qualche foglio non è nell'array restituito, il foglio non verrà caricato.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [start_sheet(sheet)](/cells/it/python-net/aspose.cells/loadfilter/start_sheet/#Worksheet) | Prepara le opzioni di filtro prima di caricare un determinato foglio di lavoro.<br/>L'implementazione dell'utente di LoadFilter può modificare LoadDataFilterOptions qui<br/> per indicare come caricare i dati per questo foglio di lavoro.|



###  Osservazioni

L'utente può specificare le opzioni di filtro o implementare il proprio LoadFilter per specificare come caricare i dati.

###  Guarda anche
* modulo [aspose.cells](..)
