---
title: classe PdfSaveOptions
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 1180
url: /it/python-net/aspose.cells/pdfsaveoptions/
is_root: false
---
##  classe PdfSaveOptions
Rappresenta le opzioni per il salvataggio del file pdf.



**Eredità:** [PdfSaveOptions](/cells/python-net/aspose.cells/pdfsaveoptions) → 
[PaginatedSaveOptions](/cells/python-net/aspose.cells/paginatedsaveoptions) → 
[SaveOptions](/cells/it/python-net/aspose.cells/saveoptions)



Il tipo PdfSaveOptions espone i membri seguenti:

###  Costruttori
| Costruttore| Descrizione|
| :- | :- |
| [PdfSaveOptions()](/cells/it/python-net/aspose.cells/pdfsaveoptions/__init__/#) | Crea le opzioni per il salvataggio del file pdf.|


###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [save_format](/cells/it/python-net/aspose.cells/pdfsaveoptions/save_format) | Ottiene il formato del file di salvataggio.|
| [clear_data](/cells/it/python-net/aspose.cells/pdfsaveoptions/clear_data) | Rendi vuota la cartella di lavoro dopo aver salvato il file.|
| [cached_file_folder](/cells/it/python-net/aspose.cells/pdfsaveoptions/cached_file_folder) | La cartella dei file memorizzati nella cache viene utilizzata per archiviare alcuni dati di grandi dimensioni.|
| [validate_merged_areas](/cells/it/python-net/aspose.cells/pdfsaveoptions/validate_merged_areas) | Indica se convalidare le celle unite prima di salvare il file.|
| [merge_areas](/cells/it/python-net/aspose.cells/pdfsaveoptions/merge_areas) | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file.|
| [create_directory](/cells/it/python-net/aspose.cells/pdfsaveoptions/create_directory) | Se true e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file.|
| [sort_names](/cells/it/python-net/aspose.cells/pdfsaveoptions/sort_names) | Indica se ordinare i nomi definiti prima di salvare il file.|
| [sort_external_names](/cells/it/python-net/aspose.cells/pdfsaveoptions/sort_external_names) | Indica se ordinare i nomi definiti esterni prima di salvare il file.|
| [refresh_chart_cache](/cells/it/python-net/aspose.cells/pdfsaveoptions/refresh_chart_cache) |Indica se aggiornare i dati della cache del grafico|
| [warning_callback](/cells/it/python-net/aspose.cells/pdfsaveoptions/warning_callback) | Ottiene o imposta la richiamata di avviso.|
| [update_smart_art](/cells/it/python-net/aspose.cells/pdfsaveoptions/update_smart_art) | Indica se aggiornare l'impostazione della grafica intelligente.<br/> Il valore predefinito è falso.|
| [default_font](/cells/it/python-net/aspose.cells/pdfsaveoptions/default_font) | Quando i caratteri in Excel sono Unicode e non devono essere impostati con il carattere corretto nello stile della cella,<br/>Possono apparire come blocco in pdf, immagine.<br/>Imposta il DefaultFont come MingLiu o MS Gothic per mostrare questi caratteri.<br/> Se questa proprietà non è impostata, Aspose.Cells utilizzerà il carattere predefinito del sistema per mostrare questi caratteri Unicode.|
| [check_workbook_default_font](/cells/it/python-net/aspose.cells/pdfsaveoptions/check_workbook_default_font) | Quando i caratteri in Excel sono Unicode e non devono essere impostati con il carattere corretto nello stile della cella,<br/>Possono apparire come blocco in pdf, immagine.<br/> Imposta questo su true per provare a utilizzare il carattere predefinito della cartella di lavoro per mostrare prima questi caratteri.|
| [check_font_compatibility](/cells/it/python-net/aspose.cells/pdfsaveoptions/check_font_compatibility) | Indica se controllare la compatibilità dei caratteri per ogni carattere nel testo.|
| [is_font_substitution_char_granularity](/cells/it/python-net/aspose.cells/pdfsaveoptions/is_font_substitution_char_granularity) | Indica se sostituire il font del carattere solo quando il font della cella non è compatibile con esso.|
| [one_page_per_sheet](/cells/it/python-net/aspose.cells/pdfsaveoptions/one_page_per_sheet) | Se OnePagePerSheet è true , tutto il contenuto di un foglio verrà restituito a una sola pagina nel risultato.<br/> Il formato carta di pagesetup non sarà valido e le altre impostazioni di pagesetup<br/> avrà ancora effetto.|
| [all_columns_in_one_page_per_sheet](/cells/it/python-net/aspose.cells/pdfsaveoptions/all_columns_in_one_page_per_sheet) | Se AllColumnsInOnePagePerSheet è true , tutto il contenuto della colonna di un foglio verrà restituito a una sola pagina nel risultato.<br/> La larghezza del formato carta di pagesetup verrà ignorata e le altre impostazioni di pagesetup<br/> avrà ancora effetto.|
| [ignore_error](/cells/it/python-net/aspose.cells/pdfsaveoptions/ignore_error) | Indica se è necessario nascondere l'errore durante il rendering.<br/> L'errore può essere un errore nella forma, nell'immagine, nel rendering del grafico, ecc.|
| [output_blank_page_when_nothing_to_print](/cells/it/python-net/aspose.cells/pdfsaveoptions/output_blank_page_when_nothing_to_print) | Indica se emettere una pagina vuota quando non c'è niente da stampare.|
| [page_index](/cells/it/python-net/aspose.cells/pdfsaveoptions/page_index) | Ottiene o imposta l'indice in base 0 della prima pagina da salvare.|
| [page_count](/cells/it/python-net/aspose.cells/pdfsaveoptions/page_count) | Ottiene o imposta il numero di pagine da salvare.|
| [printing_page_type](/cells/it/python-net/aspose.cells/pdfsaveoptions/printing_page_type) | Indica quali pagine non verranno stampate.|
| [gridline_type](/cells/it/python-net/aspose.cells/pdfsaveoptions/gridline_type) | Ottiene o imposta il tipo di griglia.|
| [text_cross_type](/cells/it/python-net/aspose.cells/pdfsaveoptions/text_cross_type) | Ottiene o imposta la visualizzazione del tipo di testo quando la larghezza del testo è maggiore della larghezza della cella.|
| [default_edit_language](/cells/it/python-net/aspose.cells/pdfsaveoptions/default_edit_language) | Ottiene o imposta la lingua di modifica predefinita.|
| [sheet_set](/cells/it/python-net/aspose.cells/pdfsaveoptions/sheet_set) |Ottiene o imposta i fogli di cui eseguire il rendering. L'impostazione predefinita è tutti i fogli visibili nella cartella di lavoro: [SheetSet.visible](/cells/it/python-net/aspose.cells.rendering/sheetset#visible).|
| [draw_object_event_handler](/cells/it/python-net/aspose.cells/pdfsaveoptions/draw_object_event_handler) | Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering.|
| [page_saving_callback](/cells/it/python-net/aspose.cells/pdfsaveoptions/page_saving_callback) |Controlla/Indica l'avanzamento del processo di salvataggio della pagina.|
| [embed_standard_windows_fonts](/cells/it/python-net/aspose.cells/pdfsaveoptions/embed_standard_windows_fonts) | True per incorporare font true type.<br/>Interessa solo i caratteri ASCII 32-127.<br/>I caratteri per i codici di caratteri superiori a 127 sono sempre incorporati.<br/>I caratteri sono sempre incorporati per lo standard PDF/A-1a, PDF/A-1b.<br/> L'impostazione predefinita è true.|
| [bookmark](/cells/it/python-net/aspose.cells/pdfsaveoptions/bookmark) | Ottiene e imposta l'oggetto [PdfBookmarkEntry](/cells/it/python-net/aspose.cells.rendering/pdfbookmarkentry).|
| [compliance](/cells/it/python-net/aspose.cells/pdfsaveoptions/compliance) | La cartella di lavoro converte in pdf secondo PdfCompliance in questa proprietà.|
| [security_options](/cells/it/python-net/aspose.cells/pdfsaveoptions/security_options) | Imposta queste opzioni, quando la sicurezza è necessaria nel risultato xls2pdf.|
| [image_type](/cells/it/python-net/aspose.cells/pdfsaveoptions/image_type) | Rappresenta il tipo di immagine durante la conversione del grafico e della forma.|
| [calculate_formula](/cells/it/python-net/aspose.cells/pdfsaveoptions/calculate_formula) | Indica se calcolare le formule prima di salvare il file pdf.|
| [pdf_compression](/cells/it/python-net/aspose.cells/pdfsaveoptions/pdf_compression) |Indicare l'algoritmo di compressione|
| [created_time](/cells/it/python-net/aspose.cells/pdfsaveoptions/created_time) | Ottiene e imposta l'ora di generazione del documento pdf.|
| [producer](/cells/it/python-net/aspose.cells/pdfsaveoptions/producer) | Ottiene e imposta il produttore del documento pdf generato.|
| [optimization_type](/cells/it/python-net/aspose.cells/pdfsaveoptions/optimization_type) | Ottiene e imposta il tipo di ottimizzazione pdf.|
| [custom_properties_export](/cells/it/python-net/aspose.cells/pdfsaveoptions/custom_properties_export) | Ottiene o imposta un valore che determina il modo in cui [CustomDocumentPropertyCollection](/cells/it/python-net/aspose.cells.properties/customdocumentpropertycollection) viene esportato nel file PDF. Il valore predefinito è Nessuno.|
| [export_document_structure](/cells/it/python-net/aspose.cells/pdfsaveoptions/export_document_structure) | Indica se esportare la struttura del documento.|
| [emf_render_setting](/cells/it/python-net/aspose.cells/pdfsaveoptions/emf_render_setting) | Impostazione per il rendering del metafile EMF.|
| [display_doc_title](/cells/it/python-net/aspose.cells/pdfsaveoptions/display_doc_title) | Indica se la barra del titolo della finestra deve visualizzare il titolo del documento.|
| [font_encoding](/cells/it/python-net/aspose.cells/pdfsaveoptions/font_encoding) | Ottiene o imposta la codifica dei caratteri incorporati in pdf.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [set_image_resample(desired_ppi, jpeg_quality)](/cells/it/python-net/aspose.cells/pdfsaveoptions/set_image_resample/#int-int) | Imposta il PPI desiderato (pixel per pollice) delle immagini di ricampionamento e la qualità jpeg.<br/> Tutte le immagini verranno convertite in JPEG con l'impostazione di qualità specificata,<br/> le immagini più grandi del PPI (pixel per pollice) specificato verranno ricampionate.|



###  Guarda anche
* modulo [aspose.cells](..)
* classe [CustomDocumentPropertyCollection](/cells/it/python-net/aspose.cells.properties/customdocumentpropertycollection)
* classe [PaginatedSaveOptions](/cells/it/python-net/aspose.cells/paginatedsaveoptions)
* classe [PdfBookmarkEntry](/cells/it/python-net/aspose.cells.rendering/pdfbookmarkentry)
* classe [PdfSaveOptions](/cells/it/python-net/aspose.cells/pdfsaveoptions)
* classe [SaveOptions](/cells/it/python-net/aspose.cells/saveoptions)
