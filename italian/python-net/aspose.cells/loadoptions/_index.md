---
title: classe LoadOptions
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 1020
url: /it/python-net/aspose.cells/loadoptions/
is_root: false
---
##  classe LoadOptions
Rappresenta le opzioni di caricamento del file.



Il tipo LoadOptions espone i membri seguenti:

###  Costruttori
| Costruttore| Descrizione|
| :- | :- |
| [LoadOptions()](/cells/it/python-net/aspose.cells/loadoptions/__init__/#) | Crea un'opzione di caricamento del file.|
| [LoadOptions(load_format)](/cells/it/python-net/aspose.cells/loadoptions/__init__/#LoadFormat) | Crea un'opzione di caricamento del file.|


###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [load_format](/cells/it/python-net/aspose.cells/loadoptions/load_format) | Ottiene il formato di caricamento.|
| [password](/cells/it/python-net/aspose.cells/loadoptions/password) | Ottiene e imposta la password della cartella di lavoro.|
| [parsing_formula_on_open](/cells/it/python-net/aspose.cells/loadoptions/parsing_formula_on_open) | Indica se analizzare la formula durante la lettura del file.|
| [parsing_pivot_cached_records](/cells/it/python-net/aspose.cells/loadoptions/parsing_pivot_cached_records) | Indica se l'analisi dei record memorizzati nella cache pivot durante il caricamento del file.<br/> Il valore predefinito è falso.|
| [language_code](/cells/it/python-net/aspose.cells/loadoptions/language_code) | Ottiene o imposta la lingua dell'interfaccia utente della versione della cartella di lavoro basata su CountryCode che ha salvato il file.|
| [region](/cells/it/python-net/aspose.cells/loadoptions/region) | Ottiene o imposta le impostazioni internazionali del sistema in base a CountryCode al momento del caricamento del file.|
| [default_style_settings](/cells/it/python-net/aspose.cells/loadoptions/default_style_settings) | Ottiene le impostazioni di stile predefinite per l'inizializzazione degli stili della cartella di lavoro|
| [standard_font](/cells/it/python-net/aspose.cells/loadoptions/standard_font) | Imposta il nome del carattere standard predefinito|
| [standard_font_size](/cells/it/python-net/aspose.cells/loadoptions/standard_font_size) | Imposta la dimensione del carattere standard predefinita.|
| [interrupt_monitor](/cells/it/python-net/aspose.cells/loadoptions/interrupt_monitor) | Ottiene e imposta il monitor di interrupt.|
| [ignore_not_printed](/cells/it/python-net/aspose.cells/loadoptions/ignore_not_printed) | Ignora i dati che non vengono stampati se stampi direttamente il file|
| [check_data_valid](/cells/it/python-net/aspose.cells/loadoptions/check_data_valid) | Verificare se i dati sono validi nel file modello.|
| [check_excel_restriction](/cells/it/python-net/aspose.cells/loadoptions/check_excel_restriction) | Se controllare la restrizione del file excel quando l'utente modifica gli oggetti relativi alle celle.<br/>Ad esempio, Excel non consente di inserire un valore di stringa più lungo di 32K.<br/>Quando inserisci un valore più lungo di 32K, ad esempio Cell.PutValue(string), se questa proprietà è true, otterrai un'eccezione.<br/>Se questa proprietà è falsa, accetteremo il valore della stringa di input come valore della cella in modo che in seguito<br/>puoi emettere il valore di stringa completo per altri formati di file come CSV.<br/>Tuttavia, se hai impostato un tipo di valore non valido per il formato di file excel,<br/> non dovresti salvare la cartella di lavoro come formato di file excel in un secondo momento. Altrimenti potrebbe esserci un errore imprevisto per il file excel generato.|
| [keep_unparsed_data](/cells/it/python-net/aspose.cells/loadoptions/keep_unparsed_data) |Se conservare i dati non analizzati in memoria per la cartella di lavoro quando viene caricata dal file modello. L'impostazione predefinita è true.|
| [load_filter](/cells/it/python-net/aspose.cells/loadoptions/load_filter) | Il filtro per indicare come caricare i dati.|
| [light_cells_data_handler](/cells/it/python-net/aspose.cells/loadoptions/light_cells_data_handler) | Il gestore dati per l'elaborazione dei dati delle celle durante la lettura del file modello.|
| [memory_setting](/cells/it/python-net/aspose.cells/loadoptions/memory_setting) | Ottiene o imposta le opzioni di utilizzo della memoria.|
| [warning_callback](/cells/it/python-net/aspose.cells/loadoptions/warning_callback) | Ottiene o imposta la richiamata di avviso.|
| [auto_fitter_options](/cells/it/python-net/aspose.cells/loadoptions/auto_fitter_options) | Ottiene e imposta le opzioni di installazione automatica|
| [auto_filter](/cells/it/python-net/aspose.cells/loadoptions/auto_filter) | Indica se filtrare automaticamente i dati durante il caricamento dei file.|
| [font_configs](/cells/it/python-net/aspose.cells/loadoptions/font_configs) | Ottiene e imposta le singole configurazioni dei caratteri.<br/> Funziona solo per [Workbook](/cells/it/python-net/aspose.cells/workbook) che utilizza questo [LoadOptions](/cells/it/python-net/aspose.cells/loadoptions) per caricare.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [set_paper_size(type)](/cells/it/python-net/aspose.cells/loadoptions/set_paper_size/#PaperSizeType) | Imposta il formato carta di stampa predefinito dall'impostazione predefinita della stampante.|



###  Guarda anche
* modulo [aspose.cells](..)
* classe [LoadOptions](/cells/it/python-net/aspose.cells/loadoptions)
* classe [Workbook](/cells/it/python-net/aspose.cells/workbook)
