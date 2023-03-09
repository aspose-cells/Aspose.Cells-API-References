---
title: classe Workbook
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 1590
url: /it/python-net/aspose.cells/workbook/
is_root: false
---
##  classe Workbook
Rappresenta un oggetto radice per creare un foglio di calcolo Excel.



Il tipo Workbook espone i membri seguenti:

###  Costruttori
| Costruttore| Descrizione|
| :- | :- |
| [Workbook()](/cells/it/python-net/aspose.cells/workbook/__init__/#) | Inizializza una nuova istanza della classe [Workbook](/cells/it/python-net/aspose.cells/workbook).|
| [Workbook(file_format_type)](/cells/it/python-net/aspose.cells/workbook/__init__/#FileFormatType) | Inizializza una nuova istanza della classe [Workbook](/cells/it/python-net/aspose.cells/workbook).|
| [Workbook(file)](/cells/it/python-net/aspose.cells/workbook/__init__/#str) | Inizializza una nuova istanza della classe [Workbook](/cells/it/python-net/aspose.cells/workbook) e apre un file.|
| [Workbook(stream)](/cells/it/python-net/aspose.cells/workbook/__init__/#io.RawIOBase) | Inizializza una nuova istanza della classe [Workbook](/cells/it/python-net/aspose.cells/workbook) e apre un flusso.|
| [Workbook(file, load_options)](/cells/it/python-net/aspose.cells/workbook/__init__/#str-LoadOptions) | Inizializza una nuova istanza della classe [Workbook](/cells/it/python-net/aspose.cells/workbook) e apre un file.|
| [Workbook(stream, load_options)](/cells/it/python-net/aspose.cells/workbook/__init__/#io.RawIOBase-LoadOptions) | Inizializza una nuova istanza della classe [Workbook](/cells/it/python-net/aspose.cells/workbook) e apre il flusso.|


###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [settings](/cells/it/python-net/aspose.cells/workbook/settings) | Rappresenta le impostazioni della cartella di lavoro.|
| [worksheets](/cells/it/python-net/aspose.cells/workbook/worksheets) | Ottiene la raccolta [WorksheetCollection](/cells/it/python-net/aspose.cells/worksheetcollection) nel foglio di calcolo.|
| [is_licensed](/cells/it/python-net/aspose.cells/workbook/is_licensed) | Indica se la licenza è impostata.|
| [colors](/cells/it/python-net/aspose.cells/workbook/colors) | Restituisce i colori nella tavolozza per il foglio di calcolo.|
| [count_of_styles_in_pool](/cells/it/python-net/aspose.cells/workbook/count_of_styles_in_pool) | Ottiene il numero degli stili nel pool di stili.|
| [default_style](/cells/it/python-net/aspose.cells/workbook/default_style) | Ottiene o imposta l'oggetto [Style](/cells/it/python-net/aspose.cells/style) predefinito della cartella di lavoro.|
| [is_digitally_signed](/cells/it/python-net/aspose.cells/workbook/is_digitally_signed) | Indica se questo foglio di calcolo è firmato digitalmente.|
| [is_workbook_protected_with_password](/cells/it/python-net/aspose.cells/workbook/is_workbook_protected_with_password) |Indica se la struttura o la finestra è protetta da password.|
| [vba_project](/cells/it/python-net/aspose.cells/workbook/vba_project) | Ottiene [Workbook.vba_project](/cells/it/python-net/aspose.cells/workbook#vba_project) in un foglio di calcolo.|
| [has_macro](/cells/it/python-net/aspose.cells/workbook/has_macro) | Indica se questo foglio di calcolo contiene macro/VBA.|
| [has_revisions](/cells/it/python-net/aspose.cells/workbook/has_revisions) | Ottiene se la cartella di lavoro contiene modifiche rilevate|
| [file_name](/cells/it/python-net/aspose.cells/workbook/file_name) | Ottiene e imposta il nome del file corrente.|
| [cells_data_table_factory](/cells/it/python-net/aspose.cells/workbook/cells_data_table_factory) | Ottiene il factory per la creazione di ICellsDataTable da oggetti personalizzati|
| [data_sorter](/cells/it/python-net/aspose.cells/workbook/data_sorter) | Ottiene un oggetto DataSorter per ordinare i dati.|
| [theme](/cells/it/python-net/aspose.cells/workbook/theme) | Ottiene il nome del tema.|
| [built_in_document_properties](/cells/it/python-net/aspose.cells/workbook/built_in_document_properties) | Restituisce una raccolta [DocumentProperty](/cells/it/python-net/aspose.cells.properties/documentproperty) che rappresenta tutte le proprietà del documento predefinite del foglio di calcolo.|
| [custom_document_properties](/cells/it/python-net/aspose.cells/workbook/custom_document_properties) | Restituisce una raccolta [DocumentProperty](/cells/it/python-net/aspose.cells.properties/documentproperty) che rappresenta tutte le proprietà del documento personalizzato del foglio di calcolo.|
| [file_format](/cells/it/python-net/aspose.cells/workbook/file_format) |Ottiene e imposta il formato del file.|
| [interrupt_monitor](/cells/it/python-net/aspose.cells/workbook/interrupt_monitor) | Ottiene e imposta il monitor di interrupt.|
| [content_type_properties](/cells/it/python-net/aspose.cells/workbook/content_type_properties) | Ottiene l'elenco di oggetti [ContentTypeProperty](/cells/it/python-net/aspose.cells.properties/contenttypeproperty) nella cartella di lavoro.|
| [custom_xml_parts](/cells/it/python-net/aspose.cells/workbook/custom_xml_parts) | Rappresenta una parte di archiviazione dati XML personalizzata (dati XML personalizzati all'interno di un pacchetto).|
| [data_mashup](/cells/it/python-net/aspose.cells/workbook/data_mashup) | Ottiene i dati di mashup.|
| [ribbon_xml](/cells/it/python-net/aspose.cells/workbook/ribbon_xml) | Ottiene e imposta il file XML che definisce l'interfaccia utente della barra multifunzione.|
| [absolute_path](/cells/it/python-net/aspose.cells/workbook/absolute_path) | Ottiene e imposta il percorso assoluto del file.|
| [data_connections](/cells/it/python-net/aspose.cells/workbook/data_connections) | Ottiene la raccolta [ExternalConnection](/cells/it/python-net/aspose.cells.externalconnections/externalconnection).|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [save(file_name, save_format)](/cells/it/python-net/aspose.cells/workbook/save/#str-SaveFormat) | Salva la cartella di lavoro sul disco.|
| [save(file_name)](/cells/it/python-net/aspose.cells/workbook/save/#str) | Salva la cartella di lavoro sul disco.|
| [save(file_name, save_options)](/cells/it/python-net/aspose.cells/workbook/save/#str-SaveOptions) | Salva la cartella di lavoro sul disco.|
| [save(stream, save_format)](/cells/it/python-net/aspose.cells/workbook/save/#io.RawIOBase-SaveFormat) | Salva la cartella di lavoro nel flusso.|
| [save(stream, save_options)](/cells/it/python-net/aspose.cells/workbook/save/#io.RawIOBase-SaveOptions) | Salva la cartella di lavoro nel flusso.|
| [replace(place_holder, new_value)](/cells/it/python-net/aspose.cells/workbook/replace/#str-str) | Sostituisce il valore di una cella con una nuova stringa.|
| [replace(place_holder, new_value)](/cells/it/python-net/aspose.cells/workbook/replace/#str-int) |Sostituisce il valore di una cella con un nuovo numero intero.|
| [replace(place_holder, new_value)](/cells/it/python-net/aspose.cells/workbook/replace/#str-float) | Sostituisce il valore di una cella con un nuovo double.|
| [replace(place_holder, new_values, is_vertical)](/cells/it/python-net/aspose.cells/workbook/replace/#str-list-bool) | Sostituisce il valore di una cella con un nuovo array di stringhe.|
| [replace(place_holder, new_values, is_vertical)](/cells/it/python-net/aspose.cells/workbook/replace/#str-list-bool) | Sostituisce i valori delle celle con un array di interi.|
| [replace(place_holder, new_values, is_vertical)](/cells/it/python-net/aspose.cells/workbook/replace/#str-list-bool) | Sostituisce i valori delle celle con un doppio array.|
| [replace(bool_value, new_value)](/cells/it/python-net/aspose.cells/workbook/replace/#bool-any) | Sostituisce i valori delle celle con nuovi dati.|
| [replace(int_value, new_value)](/cells/it/python-net/aspose.cells/workbook/replace/#int-any) | Sostituisce i valori delle celle con nuovi dati.|
| [replace(place_holder, new_value, options)](/cells/it/python-net/aspose.cells/workbook/replace/#str-str-ReplaceOptions) | Sostituisce il valore di una cella con una nuova stringa.|
| [copy(source, copy_options)](/cells/it/python-net/aspose.cells/workbook/copy/#Workbook-CopyOptions) |Copia i dati da un oggetto Workbook di origine.|
| [copy(source)](/cells/it/python-net/aspose.cells/workbook/copy/#Workbook) |Copia i dati da un oggetto Workbook di origine.|
| [calculate_formula()](/cells/it/python-net/aspose.cells/workbook/calculate_formula/#) | Calcola il risultato delle formule.|
| [calculate_formula(ignore_error)](/cells/it/python-net/aspose.cells/workbook/calculate_formula/#bool) | Calcola il risultato delle formule.|
| [calculate_formula(ignore_error, custom_function)](/cells/it/python-net/aspose.cells/workbook/calculate_formula/#bool-ICustomFunction) | Calcola il risultato delle formule.|
| [calculate_formula(options)](/cells/it/python-net/aspose.cells/workbook/calculate_formula/#CalculationOptions) | Calcolo delle formule in questa cartella di lavoro.|
| [refresh_dynamic_array_formulas(calculate)](/cells/it/python-net/aspose.cells/workbook/refresh_dynamic_array_formulas/#bool) | Aggiorna le formule di matrice dinamica (si riversa in un nuovo intervallo di celle vicine in base ai dati correnti)<br/> Altre formule nella cartella di lavoro non verranno calcolate in modo ricorsivo anche se sono state utilizzate da formule di matrice dinamica.|
| [refresh_dynamic_array_formulas(calculate, copts)](/cells/it/python-net/aspose.cells/workbook/refresh_dynamic_array_formulas/#bool-CalculationOptions) | Aggiorna le formule di matrice dinamica (si riversa in un nuovo intervallo di celle vicine in base ai dati correnti)|
| [import_xml(url, sheet_name, row, col)](/cells/it/python-net/aspose.cells/workbook/import_xml/#str-str-int-int) | Importa/aggiorna un file di dati XML nella cartella di lavoro.|
| [import_xml(stream, sheet_name, row, col)](/cells/it/python-net/aspose.cells/workbook/import_xml/#io.RawIOBase-str-int-int) | Importa/aggiorna un file di dati XML nella cartella di lavoro.|
| [export_xml(map_name, path)](/cells/it/python-net/aspose.cells/workbook/export_xml/#str-str) | Esporta i dati XML collegati dalla mappa XML specificata.|
| [export_xml(map_name, stream)](/cells/it/python-net/aspose.cells/workbook/export_xml/#str-io.RawIOBase) | Esporta dati XML.|
| [parse_formulas(ignore_error)](/cells/it/python-net/aspose.cells/workbook/parse_formulas/#bool) | Analizza tutte le formule che non sono state analizzate quando sono state caricate da un file modello o impostate su una cella.|
| [start_access_cache(opts)](/cells/it/python-net/aspose.cells/workbook/start_access_cache/#AccessCacheOptions) | Avvia la sessione che utilizza le cache per accedere ai dati.|
| [close_access_cache(opts)](/cells/it/python-net/aspose.cells/workbook/close_access_cache/#AccessCacheOptions) | Chiude la sessione che utilizza le cache per accedere ai dati.|
| [remove_unused_styles()](/cells/it/python-net/aspose.cells/workbook/remove_unused_styles/#) | Rimuovi tutti gli stili inutilizzati.|
| [create_style()](/cells/it/python-net/aspose.cells/workbook/create_style/#) |Crea un nuovo stile.|
| [create_builtin_style(type)](/cells/it/python-net/aspose.cells/workbook/create_builtin_style/#BuiltinStyleType) | Crea uno stile integrato in base al tipo specificato.|
| [create_cells_color()](/cells/it/python-net/aspose.cells/workbook/create_cells_color/#) | Crea un oggetto [CellsColor](/cells/it/python-net/aspose.cells/cellscolor).|
| [combine(second_workbook)](/cells/it/python-net/aspose.cells/workbook/combine/#Workbook) | Combina un altro oggetto cartella di lavoro.|
| [get_style_in_pool(index)](/cells/it/python-net/aspose.cells/workbook/get_style_in_pool/#int) | Ottiene lo stile nel pool di stili.<br/>Tutti gli stili nella cartella di lavoro verranno raccolti in un pool.<br/> C'è solo un semplice indice di riferimento nelle celle.|
| [get_fonts()](/cells/it/python-net/aspose.cells/workbook/get_fonts/#) | Ottiene tutti i tipi di carattere nel pool di stili.|
| [get_named_style(name)](/cells/it/python-net/aspose.cells/workbook/get_named_style/#str) | Ottiene lo stile denominato nel pool di stili.|
| [change_palette(color, index)](/cells/it/python-net/aspose.cells/workbook/change_palette/#aspose.pydrawing.Color-int) | Modifica la tavolozza per il foglio di calcolo nell'indice specificato.|
| [is_color_in_palette(color)](/cells/it/python-net/aspose.cells/workbook/is_color_in_palette/#aspose.pydrawing.Color) | Controlla se un colore è nella tavolozza per il foglio di calcolo.|
| [get_matching_color(raw_color)](/cells/it/python-net/aspose.cells/workbook/get_matching_color/#aspose.pydrawing.Color) | Trova il miglior colore corrispondente nella tavolozza corrente.|
| [set_encryption_options(encryption_type, key_length)](/cells/it/python-net/aspose.cells/workbook/set_encryption_options/#EncryptionType-int) | Imposta le opzioni di crittografia.|
| [protect(protection_type, password)](/cells/it/python-net/aspose.cells/workbook/protect/#ProtectionType-str) | Protegge una cartella di lavoro.|
| [protect_shared_workbook(password)](/cells/it/python-net/aspose.cells/workbook/protect_shared_workbook/#str) | Protegge una cartella di lavoro condivisa.|
| [unprotect(password)](/cells/it/python-net/aspose.cells/workbook/unprotect/#str) | Sprotegge una cartella di lavoro.|
| [unprotect_shared_workbook(password)](/cells/it/python-net/aspose.cells/workbook/unprotect_shared_workbook/#str) | Sprotegge una cartella di lavoro condivisa.|
| [remove_macro()](/cells/it/python-net/aspose.cells/workbook/remove_macro/#) | Rimuove VBA/macro da questo foglio di calcolo.|
| [remove_digital_signature()](/cells/it/python-net/aspose.cells/workbook/remove_digital_signature/#) | Rimuove la firma digitale da questo foglio di lavoro.|
| [accept_all_revisions()](/cells/it/python-net/aspose.cells/workbook/accept_all_revisions/#) | Accetta tutte le modifiche rilevate nella cartella di lavoro.|
| [remove_external_links()](/cells/it/python-net/aspose.cells/workbook/remove_external_links/#) | Rimuove tutti i collegamenti esterni nella cartella di lavoro.|
| [get_theme_color(type)](/cells/it/python-net/aspose.cells/workbook/get_theme_color/#ThemeColorType) | Ottiene il colore del tema.|
| [set_theme_color(type, color)](/cells/it/python-net/aspose.cells/workbook/set_theme_color/#ThemeColorType-aspose.pydrawing.Color) | Imposta il colore del tema|
| [custom_theme(theme_name, colors)](/cells/it/python-net/aspose.cells/workbook/custom_theme/#str-aspose.pydrawing.Color[]) | Personalizza il tema.|
| [copy_theme(source)](/cells/it/python-net/aspose.cells/workbook/copy_theme/#Workbook) | Copia il tema da un'altra cartella di lavoro.|
| [has_exernal_links()](/cells/it/python-net/aspose.cells/workbook/has_exernal_links/#) | Indica se questa cartella di lavoro contiene collegamenti esterni ad altre origini dati.|
| [update_linked_data_source(external_workbooks)](/cells/it/python-net/aspose.cells/workbook/update_linked_data_source/#list) | Se questa cartella di lavoro contiene collegamenti esterni ad un'altra origine dati,<br/>Aspose.Cells tenterà di recuperare i dati più recenti.|
| [set_digital_signature(digital_signature_collection)](/cells/it/python-net/aspose.cells/workbook/set_digital_signature/#aspose.cells.digitalsignatures.DigitalSignatureCollection) | Imposta la firma digitale su un file di foglio di calcolo (Excel2007 e versioni successive).|
| [add_digital_signature(digital_signature_collection)](/cells/it/python-net/aspose.cells/workbook/add_digital_signature/#aspose.cells.digitalsignatures.DigitalSignatureCollection) | Aggiunge la firma digitale a un file di foglio di calcolo OOXML (Excel2007 e versioni successive).|
| [get_digital_signature()](/cells/it/python-net/aspose.cells/workbook/get_digital_signature/#) | Ottiene la firma digitale dal file.|
| [remove_personal_information()](/cells/it/python-net/aspose.cells/workbook/remove_personal_information/#) | Rimuove le informazioni personali.|



###  Osservazioni

La classe Workbook denota un foglio di calcolo Excel. Ogni foglio di calcolo può contenere più fogli di lavoro.
La caratteristica di base della classe è aprire e salvare file excel nativi.
La classe ha alcune funzionalità avanzate come la copia dei dati da altre cartelle di lavoro, la combinazione di due cartelle di lavoro e la protezione del foglio di calcolo Excel.

###  Esempio

 L'esempio seguente carica un Workbook da un file denominato designer.xls e rende invisibili le barre di scorrimento orizzontale e verticale per Workbook. Quindi sostituisce due valori stringa rispettivamente con un valore intero e un valore stringa all'interno del foglio di calcolo e infine invia il file aggiornato a il navigatore del cliente.

```python
from aspose.cells import Workbook

# Open a designer file
designerFile = "designer.xls"
workbook = Workbook(designerFile)
# Set scroll bars
workbook.settings.is_h_scroll_bar_visible = False
workbook.settings.is_v_scroll_bar_visible = False
# Replace the placeholder string with new values
newInt = 100
workbook.replace("OldInt", newInt)
newString = "Hello!"
workbook.replace("OldString", newString)
workbook.save("result.xls")

```

###  Guarda anche
* modulo [aspose.cells](..)
* classe [CellsColor](/cells/it/python-net/aspose.cells/cellscolor)
* classe [ContentTypeProperty](/cells/it/python-net/aspose.cells.properties/contenttypeproperty)
* classe [DocumentProperty](/cells/it/python-net/aspose.cells.properties/documentproperty)
* classe [ExternalConnection](/cells/it/python-net/aspose.cells.externalconnections/externalconnection)
* classe [Style](/cells/it/python-net/aspose.cells/style)
* classe [Workbook](/cells/it/python-net/aspose.cells/workbook)
* classe [WorksheetCollection](/cells/it/python-net/aspose.cells/worksheetcollection)
