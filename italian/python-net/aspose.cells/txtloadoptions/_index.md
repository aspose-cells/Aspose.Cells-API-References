---
title: classe TxtLoadOptions
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 1510
url: /it/python-net/aspose.cells/txtloadoptions/
is_root: false
---
##  classe TxtLoadOptions
Rappresenta le opzioni per il caricamento del file di testo.



**Eredità:** [TxtLoadOptions](/cells/python-net/aspose.cells/txtloadoptions) → 
[AbstractTextLoadOptions](/cells/python-net/aspose.cells/abstracttextloadoptions) → 
[LoadOptions](/cells/it/python-net/aspose.cells/loadoptions)



Il tipo TxtLoadOptions espone i membri seguenti:

###  Costruttori
| Costruttore| Descrizione|
| :- | :- |
| [TxtLoadOptions()](/cells/it/python-net/aspose.cells/txtloadoptions/__init__/#) | Crea le opzioni per il caricamento del file di testo.|
| [TxtLoadOptions(load_format)](/cells/it/python-net/aspose.cells/txtloadoptions/__init__/#LoadFormat) | Crea le opzioni per il caricamento del file di testo.|


###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [load_format](/cells/it/python-net/aspose.cells/txtloadoptions/load_format) | Ottiene il formato di caricamento.|
| [password](/cells/it/python-net/aspose.cells/txtloadoptions/password) | Ottiene e imposta la password della cartella di lavoro.|
| [parsing_formula_on_open](/cells/it/python-net/aspose.cells/txtloadoptions/parsing_formula_on_open) | Indica se analizzare la formula durante la lettura del file.|
| [parsing_pivot_cached_records](/cells/it/python-net/aspose.cells/txtloadoptions/parsing_pivot_cached_records) | Indica se l'analisi dei record memorizzati nella cache pivot durante il caricamento del file.<br/> Il valore predefinito è falso.|
| [language_code](/cells/it/python-net/aspose.cells/txtloadoptions/language_code) | Ottiene o imposta la lingua dell'interfaccia utente della versione della cartella di lavoro basata su CountryCode che ha salvato il file.|
| [region](/cells/it/python-net/aspose.cells/txtloadoptions/region) | Ottiene o imposta le impostazioni internazionali del sistema in base a CountryCode al momento del caricamento del file.|
| [default_style_settings](/cells/it/python-net/aspose.cells/txtloadoptions/default_style_settings) | Ottiene le impostazioni di stile predefinite per l'inizializzazione degli stili della cartella di lavoro|
| [standard_font](/cells/it/python-net/aspose.cells/txtloadoptions/standard_font) | Imposta il nome del carattere standard predefinito|
| [standard_font_size](/cells/it/python-net/aspose.cells/txtloadoptions/standard_font_size) | Imposta la dimensione del carattere standard predefinita.|
| [interrupt_monitor](/cells/it/python-net/aspose.cells/txtloadoptions/interrupt_monitor) | Ottiene e imposta il monitor di interrupt.|
| [ignore_not_printed](/cells/it/python-net/aspose.cells/txtloadoptions/ignore_not_printed) | Ignora i dati che non vengono stampati se stampi direttamente il file|
| [check_data_valid](/cells/it/python-net/aspose.cells/txtloadoptions/check_data_valid) | Verificare se i dati sono validi nel file modello.|
| [check_excel_restriction](/cells/it/python-net/aspose.cells/txtloadoptions/check_excel_restriction) | Se controllare la restrizione del file excel quando l'utente modifica gli oggetti relativi alle celle.<br/>Ad esempio, Excel non consente di inserire un valore di stringa più lungo di 32K.<br/>Quando inserisci un valore più lungo di 32K, ad esempio Cell.PutValue(string), se questa proprietà è true, otterrai un'eccezione.<br/>Se questa proprietà è falsa, accetteremo il valore della stringa di input come valore della cella in modo che in seguito<br/>puoi emettere il valore di stringa completo per altri formati di file come CSV.<br/>Tuttavia, se hai impostato un tipo di valore non valido per il formato di file excel,<br/> non dovresti salvare la cartella di lavoro come formato di file excel in un secondo momento. Altrimenti potrebbe esserci un errore imprevisto per il file excel generato.|
| [keep_unparsed_data](/cells/it/python-net/aspose.cells/txtloadoptions/keep_unparsed_data) |Se conservare i dati non analizzati in memoria per la cartella di lavoro quando viene caricata dal file modello. L'impostazione predefinita è true.|
| [load_filter](/cells/it/python-net/aspose.cells/txtloadoptions/load_filter) | Il filtro per indicare come caricare i dati.|
| [light_cells_data_handler](/cells/it/python-net/aspose.cells/txtloadoptions/light_cells_data_handler) | Il gestore dati per l'elaborazione dei dati delle celle durante la lettura del file modello.|
| [memory_setting](/cells/it/python-net/aspose.cells/txtloadoptions/memory_setting) | Ottiene o imposta le opzioni di utilizzo della memoria.|
| [warning_callback](/cells/it/python-net/aspose.cells/txtloadoptions/warning_callback) | Ottiene o imposta la richiamata di avviso.|
| [auto_fitter_options](/cells/it/python-net/aspose.cells/txtloadoptions/auto_fitter_options) | Ottiene e imposta le opzioni di installazione automatica|
| [auto_filter](/cells/it/python-net/aspose.cells/txtloadoptions/auto_filter) | Indica se filtrare automaticamente i dati durante il caricamento dei file.|
| [font_configs](/cells/it/python-net/aspose.cells/txtloadoptions/font_configs) | Ottiene e imposta le singole configurazioni dei caratteri.<br/> Funziona solo per [Workbook](/cells/it/python-net/aspose.cells/workbook) che utilizza questo [LoadOptions](/cells/it/python-net/aspose.cells/loadoptions) per caricare.|
| [encoding](/cells/it/python-net/aspose.cells/txtloadoptions/encoding) | Ottiene e imposta la codifica predefinita. Si applica solo per file csv.|
| [load_style_strategy](/cells/it/python-net/aspose.cells/txtloadoptions/load_style_strategy) |Indica la strategia per applicare lo stile ai valori analizzati durante la conversione del valore stringa in numero o data/ora.|
| [convert_numeric_data](/cells/it/python-net/aspose.cells/txtloadoptions/convert_numeric_data) | Ottiene o imposta un valore che indica se la stringa nel file di testo viene convertita in dati numerici.|
| [convert_date_time_data](/cells/it/python-net/aspose.cells/txtloadoptions/convert_date_time_data) | Ottiene o imposta un valore che indica se la stringa nel file di testo viene convertita in dati di data.|
| [keep_precision](/cells/it/python-net/aspose.cells/txtloadoptions/keep_precision) | Indica se non analizzare un valore stringa se la lunghezza è 15.|
| [separator](/cells/it/python-net/aspose.cells/txtloadoptions/separator) |Ottiene e imposta il separatore di caratteri del file di testo.|
| [separator_string](/cells/it/python-net/aspose.cells/txtloadoptions/separator_string) | Ottiene e imposta un valore stringa come separatore.|
| [is_multi_encoded](/cells/it/python-net/aspose.cells/txtloadoptions/is_multi_encoded) | True significa che il file contiene diverse codifiche.|
| [preferred_parsers](/cells/it/python-net/aspose.cells/txtloadoptions/preferred_parsers) | Ottiene e imposta i parser di valori preferiti per il caricamento del file di testo.|
| [has_formula](/cells/it/python-net/aspose.cells/txtloadoptions/has_formula) | Indica se il testo è una formula se inizia con "=".|
| [has_text_qualifier](/cells/it/python-net/aspose.cells/txtloadoptions/has_text_qualifier) | Se è presente un qualificatore di testo per il valore della cella. L'impostazione predefinita è true.|
| [text_qualifier](/cells/it/python-net/aspose.cells/txtloadoptions/text_qualifier) | Specifica il qualificatore di testo per i valori delle celle. Il qualificatore predefinito è '"'.|
| [treat_consecutive_delimiters_as_one](/cells/it/python-net/aspose.cells/txtloadoptions/treat_consecutive_delimiters_as_one) |Indica se i delimitatori consecutivi devono essere trattati come uno solo.|
| [treat_quote_prefix_as_value](/cells/it/python-net/aspose.cells/txtloadoptions/treat_quote_prefix_as_value) |Indica se il segno delle virgolette singole iniziali deve essere preso come parte del valore di una cella.<br/>L'impostazione predefinita è true. Se è falso, le virgolette singole iniziali verranno rimosse dal valore della cella corrispondente<br/> e [Style.quote_prefix](/cells/it/python-net/aspose.cells/style#quote_prefix) verrà impostato come vero per la cella.|
| [extend_to_next_sheet](/cells/it/python-net/aspose.cells/txtloadoptions/extend_to_next_sheet) | Se estende i dati al foglio successivo quando le righe o le colonne di dati superano il limite.<br/>Se questa proprietàètrue, i dati extra saranno estesi al foglio successivo dietro a quello corrente (se il foglio corrente è l'ultimo,<br/>il nuovo foglio verrà aggiunto alla cartella di lavoro corrente).<br/>Se questa proprietà è false, i dati che superano il limite verranno ignorati.<br/> L'impostazione predefinita è false;|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [set_paper_size(type)](/cells/it/python-net/aspose.cells/txtloadoptions/set_paper_size/#PaperSizeType) | Imposta il formato carta di stampa predefinito dall'impostazione predefinita della stampante.|



###  Guarda anche
* modulo [aspose.cells](..)
* classe [AbstractTextLoadOptions](/cells/it/python-net/aspose.cells/abstracttextloadoptions)
* classe [LoadOptions](/cells/it/python-net/aspose.cells/loadoptions)
* classe [TxtLoadOptions](/cells/it/python-net/aspose.cells/txtloadoptions)
* classe [Workbook](/cells/it/python-net/aspose.cells/workbook)
