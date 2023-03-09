---
title: classe HtmlSaveOptions
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 780
url: /it/python-net/aspose.cells/htmlsaveoptions/
is_root: false
---
##  classe HtmlSaveOptions
Rappresenta le opzioni per salvare i file html.



**Eredità:** [HtmlSaveOptions](/cells/python-net/aspose.cells/htmlsaveoptions) → 
[SaveOptions](/cells/it/python-net/aspose.cells/saveoptions)



Il tipo HtmlSaveOptions espone i membri seguenti:

###  Costruttori
| Costruttore| Descrizione|
| :- | :- |
| [HtmlSaveOptions()](/cells/it/python-net/aspose.cells/htmlsaveoptions/__init__/#) | Crea opzioni per il salvataggio di file html.|
| [HtmlSaveOptions(format)](/cells/it/python-net/aspose.cells/htmlsaveoptions/__init__/#SaveFormat) | Crea opzioni per salvare i file htm.|


###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [save_format](/cells/it/python-net/aspose.cells/htmlsaveoptions/save_format) | Ottiene il formato del file di salvataggio.|
| [clear_data](/cells/it/python-net/aspose.cells/htmlsaveoptions/clear_data) | Rendi vuota la cartella di lavoro dopo aver salvato il file.|
| [cached_file_folder](/cells/it/python-net/aspose.cells/htmlsaveoptions/cached_file_folder) | La cartella dei file memorizzati nella cache viene utilizzata per archiviare alcuni dati di grandi dimensioni.|
| [validate_merged_areas](/cells/it/python-net/aspose.cells/htmlsaveoptions/validate_merged_areas) | Indica se convalidare le celle unite prima di salvare il file.|
| [merge_areas](/cells/it/python-net/aspose.cells/htmlsaveoptions/merge_areas) | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file.|
| [create_directory](/cells/it/python-net/aspose.cells/htmlsaveoptions/create_directory) | Se true e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file.|
| [sort_names](/cells/it/python-net/aspose.cells/htmlsaveoptions/sort_names) | Indica se ordinare i nomi definiti prima di salvare il file.|
| [sort_external_names](/cells/it/python-net/aspose.cells/htmlsaveoptions/sort_external_names) |Indica se ordinare i nomi definiti esternamente prima di salvare il file.|
| [refresh_chart_cache](/cells/it/python-net/aspose.cells/htmlsaveoptions/refresh_chart_cache) | Indica se aggiornare i dati della cache del grafico|
| [warning_callback](/cells/it/python-net/aspose.cells/htmlsaveoptions/warning_callback) | Ottiene o imposta callback di avviso.|
| [update_smart_art](/cells/it/python-net/aspose.cells/htmlsaveoptions/update_smart_art) | Indica se aggiornare l'impostazione della grafica intelligente.<br/> Il valore predefinito è falso.|
| [ignore_invisible_shapes](/cells/it/python-net/aspose.cells/htmlsaveoptions/ignore_invisible_shapes) |Indicare se esportare quelle forme non visibili|
| [page_title](/cells/it/python-net/aspose.cells/htmlsaveoptions/page_title) | Il titolo della pagina html.<br/> Solo per il salvataggio nel flusso html.|
| [attached_files_directory](/cells/it/python-net/aspose.cells/htmlsaveoptions/attached_files_directory) | La directory in cui verranno salvati i file allegati.<br/> Solo per il salvataggio nel flusso html.|
| [attached_files_url_prefix](/cells/it/python-net/aspose.cells/htmlsaveoptions/attached_files_url_prefix) | Specificare il prefisso URL dei file allegati come l'immagine nel file html.<br/> Solo per il salvataggio nel flusso html.|
| [default_font_name](/cells/it/python-net/aspose.cells/htmlsaveoptions/default_font_name) | Specifica il nome del carattere predefinito per l'esportazione di html, il carattere predefinito verrà utilizzato quando il carattere dello stile non esiste,<br/>Se questa proprietà è nulla, Aspose.Cells utilizzerà font universali che hanno la stessa famiglia del font originale,<br/> il valore predefinito è nullo.|
| [worksheet_scalable](/cells/it/python-net/aspose.cells/htmlsaveoptions/worksheet_scalable) | Indica se si esegue lo zoom avanti o indietro dell'html tramite il livello di zoom del foglio di lavoro durante il salvataggio del file in html, il valore predefinito è false.|
| [is_export_comments](/cells/it/python-net/aspose.cells/htmlsaveoptions/is_export_comments) | Indica se durante l'esportazione dei commenti durante il salvataggio del file in html, il valore predefinito è false.|
| [export_comments_type](/cells/it/python-net/aspose.cells/htmlsaveoptions/export_comments_type) | Rappresenta il tipo di esportazione dei commenti nei file html.|
| [disable_downlevel_revealed_comments](/cells/it/python-net/aspose.cells/htmlsaveoptions/disable_downlevel_revealed_comments) | Indica se disabilitare i commenti condizionali rivelati di livello inferiore durante l'esportazione del file in html, il valore predefinito è false.|
| [is_exp_image_to_temp_dir](/cells/it/python-net/aspose.cells/htmlsaveoptions/is_exp_image_to_temp_dir) | Indica se esportare i file di immagine nella directory temporanea.<br/> Solo per il salvataggio nel flusso html.|
| [image_scalable](/cells/it/python-net/aspose.cells/htmlsaveoptions/image_scalable) | Indica se si utilizza un'unità scalabile per descrivere la larghezza dell'immagine<br/>quando si utilizzano unità scalabili per descrivere la larghezza della colonna.<br/> Il valore predefinito è true.|
| [width_scalable](/cells/it/python-net/aspose.cells/htmlsaveoptions/width_scalable) |Indica se si utilizza l'unità scalabile per descrivere la larghezza della colonna durante l'esportazione del file in html.<br/> Il valore predefinito è falso.|
| [export_single_tab](/cells/it/python-net/aspose.cells/htmlsaveoptions/export_single_tab) | Indica se esportare la singola scheda quando il file ha un solo foglio di lavoro.<br/> Il valore predefinito è falso.|
| [export_images_as_base64](/cells/it/python-net/aspose.cells/htmlsaveoptions/export_images_as_base64) | Specifica se le immagini vengono salvate in formato Base64 su HTML, MHTML o EPUB.|
| [export_active_worksheet_only](/cells/it/python-net/aspose.cells/htmlsaveoptions/export_active_worksheet_only) | Indica se esportare l'intera cartella di lavoro in un file html.|
| [export_print_area_only](/cells/it/python-net/aspose.cells/htmlsaveoptions/export_print_area_only) | Indica se si esporta solo l'area di stampa in un file html.|
| [export_area](/cells/it/python-net/aspose.cells/htmlsaveoptions/export_area) | Ottiene o imposta la CellArea di esportazione del foglio di lavoro attivo corrente.<br/>Se imposti questo attributo, l'area di stampa del foglio di lavoro attivo corrente verrà omessa.<br/> Solo l'area specificata verrà esportata durante il salvataggio del file in html.|
| [parse_html_tag_in_cell](/cells/it/python-net/aspose.cells/htmlsaveoptions/parse_html_tag_in_cell) | Analizza il tag html nella cella, come, come valore della cella o come tag html, il valore predefinito è vero|
| [html_cross_string_type](/cells/it/python-net/aspose.cells/htmlsaveoptions/html_cross_string_type) | Indica se una stringa di celle incrociate verrà visualizzata allo stesso modo di MS Excel durante il salvataggio di un file Excel in formato html.<br/>Per impostazione predefinita, il valore è Predefinito, quindi, per le stringhe tra celle, c'è poca differenza tra i file html creati da Aspose.Cells e MS Excel.<br/> Ma le prestazioni per la creazione di file html di grandi dimensioni, impostando il valore su Cross sarebbero molte volte più veloci rispetto all'impostazione su Default o Fit2Cell.|
| [hidden_col_display_type](/cells/it/python-net/aspose.cells/htmlsaveoptions/hidden_col_display_type) |Colonna nascosta (la larghezza di questa colonna è 0) in excel, prima di salvarla in formato html,<br/>se HtmlHiddenColDisplayType è "Remove", la colonna nascosta non verrebbe emessa,<br/> se il valore è "Nascosto", la colonna sarebbe stata emessa, ma era nascosta, il valore predefinito è "Nascosto"|
| [hidden_row_display_type](/cells/it/python-net/aspose.cells/htmlsaveoptions/hidden_row_display_type) | Riga nascosta (l'altezza di questa riga è 0) in excel, prima di salvarla in formato html,<br/>se HtmlHiddenRowDisplayType è "Remove", la riga nascosta non verrebbe emessa,<br/> se il valore è "Nascosto", la riga sarebbe stata emessa, ma era nascosta, il valore predefinito è "Nascosto"|
| [encoding](/cells/it/python-net/aspose.cells/htmlsaveoptions/encoding) | Se non è impostato, usa Encoding.UTF8 come tipo di codifica predefinito.|
| [export_object_listener](/cells/it/python-net/aspose.cells/htmlsaveoptions/export_object_listener) | Ottiene o imposta ExportObjectListener per l'esportazione di oggetti.|
| [file_path_provider](/cells/it/python-net/aspose.cells/htmlsaveoptions/file_path_provider) | Ottiene o imposta IFilePathProvider per l'esportazione separata di Worksheet in HTML.|
| [stream_provider](/cells/it/python-net/aspose.cells/htmlsaveoptions/stream_provider) | Ottiene o imposta IStreamProvider per l'esportazione di oggetti.|
| [image_options](/cells/it/python-net/aspose.cells/htmlsaveoptions/image_options) | Ottenere l'oggetto ImageOrPrintOptions prima dell'esportazione|
| [save_as_single_file](/cells/it/python-net/aspose.cells/htmlsaveoptions/save_as_single_file) | Indica se salvare l'html come un singolo file.<br/> Il valore predefinito è falso.|
| [show_all_sheets](/cells/it/python-net/aspose.cells/htmlsaveoptions/show_all_sheets) | Indica se visualizzare tutti i fogli durante il salvataggio come singolo file html.|
| [export_page_headers](/cells/it/python-net/aspose.cells/htmlsaveoptions/export_page_headers) | Indica se esportare le intestazioni di pagina.|
| [export_page_footers](/cells/it/python-net/aspose.cells/htmlsaveoptions/export_page_footers) | Indica se esportare le intestazioni di pagina.|
| [export_hidden_worksheet](/cells/it/python-net/aspose.cells/htmlsaveoptions/export_hidden_worksheet) |Indica se esportare il contenuto nascosto del foglio di lavoro. Il valore predefinito è true.|
| [presentation_preference](/cells/it/python-net/aspose.cells/htmlsaveoptions/presentation_preference) | Indica se il file html o mht è la preferenza di presentazione.<br/>Il valore predefinito è falso.<br/> se vuoi ottenere una presentazione più bella, imposta il valore su true.|
| [cell_css_prefix](/cells/it/python-net/aspose.cells/htmlsaveoptions/cell_css_prefix) | Ottiene e imposta il prefisso del nome css, il valore predefinito è "".|
| [table_css_id](/cells/it/python-net/aspose.cells/htmlsaveoptions/table_css_id) | Ottiene e imposta il prefisso del nome di tipo css come tr,col,td e così via, sono contenuti nell'elemento table<br/> che ha l'attributo specifico TableCssId.|
| [is_full_path_link](/cells/it/python-net/aspose.cells/htmlsaveoptions/is_full_path_link) | Indica se si utilizza il collegamento del percorso completo in sheet00x.htm, filelist.xml e tabstrip.htm.<br/> Il valore predefinito è falso.|
| [export_worksheet_css_separately](/cells/it/python-net/aspose.cells/htmlsaveoptions/export_worksheet_css_separately) | Indica se esportare il css del foglio di lavoro separatamente. Il valore predefinito è false.|
| [export_similar_border_style](/cells/it/python-net/aspose.cells/htmlsaveoptions/export_similar_border_style) | Indica se esportare lo stile del bordo simile quando lo stile del bordo non è supportato dai browser.<br/>Se desideri importare il file html o mht in Excel, mantieni il valore predefinito.<br/> Il valore predefinito è falso.|
| [merge_empty_td_forcely](/cells/it/python-net/aspose.cells/htmlsaveoptions/merge_empty_td_forcely) | Indica se l'unione forzata dell'elemento TD vuoto durante l'esportazione del file in html.<br/> La dimensione del file html verrà ridotta in modo significativo dopo aver impostato il valore su true.<br/> Se vuoi importare il file html per eccellere o esportare le linee della griglia perfette quando salvi il file in html,<br/> si prega di mantenere il valore predefinito.|
| [export_cell_coordinate](/cells/it/python-net/aspose.cells/htmlsaveoptions/export_cell_coordinate) |Indica se esportare coordinate Excel di celle non vuote durante il salvataggio del file in html.<br/> Se desideri importare l'output html in Excel, mantieni il valore predefinito.|
| [export_extra_headings](/cells/it/python-net/aspose.cells/htmlsaveoptions/export_extra_headings) | Indica se esportare intestazioni aggiuntive quando la lunghezza del testo è maggiore della colonna di visualizzazione massima.<br/> Il valore predefinito è falso.|
| [export_headings](/cells/it/python-net/aspose.cells/htmlsaveoptions/export_headings) | Indica se esporta le intestazioni di riga e colonna del foglio durante il salvataggio nei file HTML.|
| [export_row_column_headings](/cells/it/python-net/aspose.cells/htmlsaveoptions/export_row_column_headings) | Indica se esporta le intestazioni di riga e colonna del foglio durante il salvataggio nei file HTML.|
| [export_formula](/cells/it/python-net/aspose.cells/htmlsaveoptions/export_formula) | Indica se esportare la formula durante il salvataggio del file in html.<br/> Se desideri importare l'output html in Excel, mantieni il valore predefinito.|
| [add_tooltip_text](/cells/it/python-net/aspose.cells/htmlsaveoptions/add_tooltip_text) | Indica se aggiungere il testo della descrizione comandi quando i dati non possono essere visualizzati completamente.<br/> Il valore predefinito è falso.|
| [export_grid_lines](/cells/it/python-net/aspose.cells/htmlsaveoptions/export_grid_lines) | Indica se esportare le linee della griglia. Il valore predefinito è false.|
| [export_bogus_row_data](/cells/it/python-net/aspose.cells/htmlsaveoptions/export_bogus_row_data) | Indica se esportare i dati della riga inferiore fasulli. Il valore predefinito è true. Se si desidera importare il file html o mht<br/> per eccellere, mantieni il valore predefinito.|
| [exclude_unused_styles](/cells/it/python-net/aspose.cells/htmlsaveoptions/exclude_unused_styles) | Indica se esclude gli stili inutilizzati.<br/>Per i file html generati, l'esclusione degli stili inutilizzati può ridurre le dimensioni del file<br/>senza influenzare gli effetti visivi.<br/>Se l'utente deve mantenere tutti gli stili nella cartella di lavoro per l'html generato (come lo scenario che user<br/>deve ripristinare successivamente la cartella di lavoro dall'html generato), impostare questa proprietà su false.|
| [export_document_properties](/cells/it/python-net/aspose.cells/htmlsaveoptions/export_document_properties) | Indica se esportare le proprietà del documento.Il valore predefinito è true.Se si desidera importare<br/> il file html o mht in Excel, mantieni il valore predefinito.|
| [export_worksheet_properties](/cells/it/python-net/aspose.cells/htmlsaveoptions/export_worksheet_properties) | Indica se esportare le proprietà del foglio di lavoro.Il valore predefinito è true.Se si desidera importare<br/> il file html o mht in Excel, mantieni il valore predefinito.|
| [export_workbook_properties](/cells/it/python-net/aspose.cells/htmlsaveoptions/export_workbook_properties) | Indica se si esportano le proprietà della cartella di lavoro. Il valore predefinito è true. Se si desidera importare<br/> il file html o mht in Excel, mantieni il valore predefinito.|
| [export_frame_scripts_and_properties](/cells/it/python-net/aspose.cells/htmlsaveoptions/export_frame_scripts_and_properties) | Indica se esportare gli script dei frame e le proprietà del documento. Il valore predefinito è true. Se si desidera importare il file html o mht<br/> per eccellere, mantieni il valore predefinito.|
| [export_data_options](/cells/it/python-net/aspose.cells/htmlsaveoptions/export_data_options) | Indica la regola di esportazione dei dati del file html. Il valore predefinito è Tutto.|
| [link_target_type](/cells/it/python-net/aspose.cells/htmlsaveoptions/link_target_type) | Indicando il tipo di attributo di destinazione in<a> link,Il valore predefinito è HtmlLinkTargetType.Parent.|



###  Guarda anche
* modulo [aspose.cells](..)
* classe [HtmlSaveOptions](/cells/it/python-net/aspose.cells/htmlsaveoptions)
* classe [SaveOptions](/cells/it/python-net/aspose.cells/saveoptions)
