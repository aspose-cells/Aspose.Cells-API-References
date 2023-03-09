---
title: classe HtmlLoadOptions
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 770
url: /it/python-net/aspose.cells/htmlloadoptions/
is_root: false
---
##  classe HtmlLoadOptions
Rappresenta le opzioni durante l'importazione di un file html.



**Eredità:** [HtmlLoadOptions](/cells/python-net/aspose.cells/htmlloadoptions) → 
[AbstractTextLoadOptions](/cells/python-net/aspose.cells/abstracttextloadoptions) → 
[LoadOptions](/cells/it/python-net/aspose.cells/loadoptions)



Il tipo HtmlLoadOptions espone i membri seguenti:

###  Costruttori
| Costruttore| Descrizione|
| :- | :- |
| [HtmlLoadOptions()](/cells/it/python-net/aspose.cells/htmlloadoptions/__init__/#) | Crea un'opzione di caricamento del file.|
| [HtmlLoadOptions(load_format)](/cells/it/python-net/aspose.cells/htmlloadoptions/__init__/#LoadFormat) | Crea un'opzione di caricamento del file.|


###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [load_format](/cells/it/python-net/aspose.cells/htmlloadoptions/load_format) | Ottiene il formato di caricamento.|
| [password](/cells/it/python-net/aspose.cells/htmlloadoptions/password) | Ottiene e imposta la password della cartella di lavoro.|
| [parsing_formula_on_open](/cells/it/python-net/aspose.cells/htmlloadoptions/parsing_formula_on_open) | Indica se analizzare la formula durante la lettura del file.|
| [parsing_pivot_cached_records](/cells/it/python-net/aspose.cells/htmlloadoptions/parsing_pivot_cached_records) | Indica se l'analisi dei record memorizzati nella cache pivot durante il caricamento del file.<br/> Il valore predefinito è falso.|
| [language_code](/cells/it/python-net/aspose.cells/htmlloadoptions/language_code) | Ottiene o imposta la lingua dell'interfaccia utente della versione della cartella di lavoro basata su CountryCode che ha salvato il file.|
| [region](/cells/it/python-net/aspose.cells/htmlloadoptions/region) | Ottiene o imposta le impostazioni internazionali del sistema in base a CountryCode al momento del caricamento del file.|
| [default_style_settings](/cells/it/python-net/aspose.cells/htmlloadoptions/default_style_settings) | Ottiene le impostazioni di stile predefinite per l'inizializzazione degli stili della cartella di lavoro|
| [standard_font](/cells/it/python-net/aspose.cells/htmlloadoptions/standard_font) | Imposta il nome del carattere standard predefinito|
| [standard_font_size](/cells/it/python-net/aspose.cells/htmlloadoptions/standard_font_size) | Imposta la dimensione del carattere standard predefinita.|
| [interrupt_monitor](/cells/it/python-net/aspose.cells/htmlloadoptions/interrupt_monitor) | Ottiene e imposta il monitor di interrupt.|
| [ignore_not_printed](/cells/it/python-net/aspose.cells/htmlloadoptions/ignore_not_printed) | Ignora i dati che non vengono stampati se stampi direttamente il file|
| [check_data_valid](/cells/it/python-net/aspose.cells/htmlloadoptions/check_data_valid) | Verificare se i dati sono validi nel file modello.|
| [check_excel_restriction](/cells/it/python-net/aspose.cells/htmlloadoptions/check_excel_restriction) | Se controllare la restrizione del file excel quando l'utente modifica gli oggetti relativi alle celle.<br/>Ad esempio, Excel non consente di inserire un valore di stringa più lungo di 32K.<br/>Quando inserisci un valore più lungo di 32K, ad esempio Cell.PutValue(string), se questa proprietà è true, otterrai un'eccezione.<br/>Se questa proprietà è falsa, accetteremo il valore della stringa di input come valore della cella in modo che in seguito<br/>puoi emettere il valore di stringa completo per altri formati di file come CSV.<br/>Tuttavia, se hai impostato un tipo di valore non valido per il formato di file excel,<br/> non dovresti salvare la cartella di lavoro come formato di file excel in un secondo momento. Altrimenti potrebbe esserci un errore imprevisto per il file excel generato.|
| [keep_unparsed_data](/cells/it/python-net/aspose.cells/htmlloadoptions/keep_unparsed_data) |Se conservare i dati non analizzati in memoria per la cartella di lavoro quando viene caricata dal file modello. L'impostazione predefinita è true.|
| [load_filter](/cells/it/python-net/aspose.cells/htmlloadoptions/load_filter) | Il filtro per indicare come caricare i dati.|
| [light_cells_data_handler](/cells/it/python-net/aspose.cells/htmlloadoptions/light_cells_data_handler) | Il gestore dati per l'elaborazione dei dati delle celle durante la lettura del file modello.|
| [memory_setting](/cells/it/python-net/aspose.cells/htmlloadoptions/memory_setting) | Ottiene o imposta le opzioni di utilizzo della memoria.|
| [warning_callback](/cells/it/python-net/aspose.cells/htmlloadoptions/warning_callback) | Ottiene o imposta la richiamata di avviso.|
| [auto_fitter_options](/cells/it/python-net/aspose.cells/htmlloadoptions/auto_fitter_options) | Ottiene e imposta le opzioni di installazione automatica|
| [auto_filter](/cells/it/python-net/aspose.cells/htmlloadoptions/auto_filter) | Indica se filtrare automaticamente i dati durante il caricamento dei file.|
| [font_configs](/cells/it/python-net/aspose.cells/htmlloadoptions/font_configs) | Ottiene e imposta le singole configurazioni dei caratteri.<br/> Funziona solo per [Workbook](/cells/it/python-net/aspose.cells/workbook) che utilizza questo [LoadOptions](/cells/it/python-net/aspose.cells/loadoptions) per caricare.|
| [encoding](/cells/it/python-net/aspose.cells/htmlloadoptions/encoding) | Ottiene e imposta la codifica predefinita. Si applica solo per file csv.|
| [load_style_strategy](/cells/it/python-net/aspose.cells/htmlloadoptions/load_style_strategy) |Indica la strategia per applicare lo stile ai valori analizzati durante la conversione del valore stringa in numero o data/ora.|
| [convert_numeric_data](/cells/it/python-net/aspose.cells/htmlloadoptions/convert_numeric_data) | Ottiene o imposta un valore che indica se la stringa nel file di testo viene convertita in dati numerici.|
| [convert_date_time_data](/cells/it/python-net/aspose.cells/htmlloadoptions/convert_date_time_data) | Ottiene o imposta un valore che indica se la stringa nel file di testo viene convertita in dati di data.|
| [keep_precision](/cells/it/python-net/aspose.cells/htmlloadoptions/keep_precision) | Indica se non analizzare un valore stringa se la lunghezza è 15.|
| [attached_files_directory](/cells/it/python-net/aspose.cells/htmlloadoptions/attached_files_directory) | La directory in cui verranno salvati i file allegati.|
| [load_formulas](/cells/it/python-net/aspose.cells/htmlloadoptions/load_formulas) | Indica se importare formule se il file html originale contiene formule|
| [support_div_tag](/cells/it/python-net/aspose.cells/htmlloadoptions/support_div_tag) | Indica se supporta il layout di<div> tag quando il file html contiene<div> tag. Il valore predefinito è falso.|
| [delete_redundant_spaces](/cells/it/python-net/aspose.cells/htmlloadoptions/delete_redundant_spaces) | Indica se eliminare gli spazi ridondanti quando il testo va a capo utilizzando le righe<br> tag.Il valore predefinito è false.|
| [auto_fit_cols_and_rows](/cells/it/python-net/aspose.cells/htmlloadoptions/auto_fit_cols_and_rows) | Indica se le colonne e le righe vengono adattate automaticamente. Il valore predefinito è falso.|
| [convert_formulas_data](/cells/it/python-net/aspose.cells/htmlloadoptions/convert_formulas_data) | se vero, converte la stringa in formula quando il valore della stringa inizia con il carattere '=', il valore predefinito è falso.|
| [stream_provider](/cells/it/python-net/aspose.cells/htmlloadoptions/stream_provider) | Ottiene o imposta StreamProviderImportHtmlFile per l'importazione di oggetti.|
| [prog_id](/cells/it/python-net/aspose.cells/htmlloadoptions/prog_id) | Ottiene l'ID del programma di creazione del file.<br/> Solo per file MHT.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [set_paper_size(type)](/cells/it/python-net/aspose.cells/htmlloadoptions/set_paper_size/#PaperSizeType) | Imposta il formato carta di stampa predefinito dall'impostazione predefinita della stampante.|



###  Guarda anche
* modulo [aspose.cells](..)
* classe [AbstractTextLoadOptions](/cells/it/python-net/aspose.cells/abstracttextloadoptions)
* classe [HtmlLoadOptions](/cells/it/python-net/aspose.cells/htmlloadoptions)
* classe [LoadOptions](/cells/it/python-net/aspose.cells/loadoptions)
* classe [Workbook](/cells/it/python-net/aspose.cells/workbook)
