---
title: classe ImageOrPrintOptions
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 40
url: /it/python-net/aspose.cells.rendering/imageorprintoptions/
is_root: false
---
##  classe ImageOrPrintOptions
Consente di specificare le opzioni durante il rendering del foglio di lavoro in immagini, la stampa del foglio di lavoro o il rendering del grafico nell'immagine.



Il tipo ImageOrPrintOptions espone i membri seguenti:

###  Costruttori
| Costruttore| Descrizione|
| :- | :- |
| [ImageOrPrintOptions()](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/__init__/#) | Costruisce una nuova istanza di ImageOrPrintOptions|


###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [save_format](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/save_format) | Ottiene o imposta il tipo di formato del file di output<br/> Supporto Tiff/XPS|
| [print_with_status_dialog](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/print_with_status_dialog) | Se PrintWithStatusDialog = true , verrà visualizzata una finestra di dialogo che mostra lo stato di stampa corrente.<br/> altrimenti non verrà visualizzata alcuna finestra di dialogo di questo tipo.|
| [horizontal_resolution](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/horizontal_resolution) |Ottiene o imposta la risoluzione orizzontale per le immagini generate, in punti per pollice.<br/> Applica il metodo di generazione dell'immagine tranne le immagini in formato Emf.|
| [vertical_resolution](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/vertical_resolution) | Ottiene o imposta la risoluzione verticale per le immagini generate, in punti per pollice.<br/> Applica il metodo di generazione dell'immagine tranne l'immagine in formato Emf.|
| [tiff_compression](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/tiff_compression) | Ottiene o imposta il tipo di compressione da applicare solo quando si salvano le pagine nel formato `Tiff`.|
| [tiff_color_depth](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/tiff_color_depth) | Ottiene o imposta la profondità di bit da applicare solo quando si salvano le pagine nel formato `Tiff`.|
| [printing_page](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/printing_page) | Indica quali pagine non verranno stampate.|
| [quality](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/quality) | Ottiene o imposta un valore che determina la qualità delle immagini generate<br/> da applicare solo quando si salvano le pagine nel formato `Jpeg`. Il valore predefinito è 100|
| [image_type](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/image_type) | Ottiene o imposta il formato delle immagini generate.<br/> valore predefinito: PNG.|
| [is_cell_auto_fit](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/is_cell_auto_fit) | Indica se la larghezza e l'altezza delle celle vengono adattate automaticamente in base al valore della cella.<br/> Il valore predefinito è falso.|
| [one_page_per_sheet](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/one_page_per_sheet) | Se OnePagePerSheet è true , tutto il contenuto di un foglio verrà restituito a una sola pagina nel risultato.<br/> Il formato carta di pagesetup non sarà valido e le altre impostazioni di pagesetup<br/> avrà ancora effetto.|
| [all_columns_in_one_page_per_sheet](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/all_columns_in_one_page_per_sheet) | Se AllColumnsInOnePagePerSheet è true , tutto il contenuto della colonna di un foglio verrà restituito a una sola pagina nel risultato.<br/> La larghezza del formato carta di pagesetup non sarà valida e le altre impostazioni di pagesetup<br/> avrà ancora effetto.|
| [draw_object_event_handler](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/draw_object_event_handler) | Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering.|
| [chart_image_type](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/chart_image_type) | Indica il tipo di immagine del grafico durante la conversione.<br/> valore predefinito: PNG.|
| [embeded_image_name_in_svg](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/embeded_image_name_in_svg) | Indica il nome file dell'immagine incorporata in svg.<br/> Questo dovrebbe essere il percorso completo con una directory come "c:\\xpsEmbedded"|
| [svg_fit_to_view_port](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/svg_fit_to_view_port) | se questa proprietà è vera, lo svg generato si adatterà alla porta di visualizzazione.|
| [only_area](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/only_area) | Se questa proprietà è true , verrà generata un'Area e nessuna scala avrà effetto.|
| [text_rendering_hint](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/text_rendering_hint) | Specifica la qualità del rendering del testo.<br/> Il valore predefinito è TextRenderingHint.SystemDefault|
| [smoothing_mode](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/smoothing_mode) | Specifica se l'attenuazione (antialiasing) viene applicata a linee e curve e ai bordi delle aree piene.<br/> Il valore predefinito è SmoothingMode.None|
| [transparent](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/transparent) | Indica se lo sfondo dell'immagine generata deve essere trasparente.|
| [pixel_format](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/pixel_format) | Ottiene o imposta il formato in pixel per le immagini generate.|
| [warning_callback](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/warning_callback) | Ottiene o imposta la richiamata di avviso.|
| [page_saving_callback](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/page_saving_callback) |Controlla/Indica l'avanzamento del processo di salvataggio della pagina.|
| [is_font_substitution_char_granularity](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/is_font_substitution_char_granularity) | Indica se sostituire il font del carattere solo quando il font della cella non è compatibile con esso.|
| [page_index](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/page_index) | Ottiene o imposta l'indice in base 0 della prima pagina da salvare.|
| [page_count](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/page_count) | Ottiene o imposta il numero di pagine da salvare.|
| [is_optimized](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/is_optimized) | Indica se ottimizzare gli elementi di output.|
| [default_font](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/default_font) | Quando i caratteri in Excel sono Unicode e non devono essere impostati con il carattere corretto nello stile della cella,<br/>Possono apparire come blocco in pdf, immagine.<br/>Imposta il DefaultFont come MingLiu o MS Gothic per mostrare questi caratteri.<br/> Se questa proprietà non è impostata, Aspose.Cells utilizzerà il carattere predefinito del sistema per mostrare questi caratteri Unicode.|
| [check_workbook_default_font](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/check_workbook_default_font) | Quando i caratteri in Excel sono Unicode e non devono essere impostati con il carattere corretto nello stile della cella,<br/>Possono apparire come blocco in pdf, immagine.<br/> Imposta questo su true per provare a utilizzare il carattere predefinito della cartella di lavoro per mostrare prima questi caratteri.|
| [output_blank_page_when_nothing_to_print](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/output_blank_page_when_nothing_to_print) | Indica se emettere una pagina vuota quando non c'è niente da stampare.|
| [gridline_type](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/gridline_type) | Ottiene o imposta il tipo di griglia.|
| [text_cross_type](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/text_cross_type) | Ottiene o imposta la visualizzazione del tipo di testo quando la larghezza del testo è maggiore della larghezza della cella.|
| [emf_type](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/emf_type) | Ottiene o imposta un EmfType che specifica il formato di Metafile..<br/>Il valore predefinito è EmfPlusDual.|
| [default_edit_language](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/default_edit_language) | Ottiene o imposta la lingua di modifica predefinita.|
| [sheet_set](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/sheet_set) |Ottiene o imposta i fogli di cui eseguire il rendering. L'impostazione predefinita è tutti i fogli visibili nella cartella di lavoro: [SheetSet.visible](/cells/it/python-net/aspose.cells.rendering/sheetset#visible).|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [set_desired_size(desired_width, desired_height)](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions/set_desired_size/#int-int) | Imposta la larghezza e l'altezza desiderate dell'immagine.|



###  Esempio

```python
from aspose.cells import Workbook
from aspose.cells.drawing import ImageType
from aspose.cells.rendering import ImageOrPrintOptions

# Set Image Or Print Options
options = ImageOrPrintOptions()
# Set output image format
options.image_type = ImageType.PNG
# Set Horizontal resolution
options.horizontal_resolution = 300
# Set Vertical Resolution
options.vertical_resolution = 300
# Instantiate Workbook
book = Workbook("test.xls")
# Save chart as Image using ImageOrPrint Options
book.worksheets[0].charts[0].to_image("chart.png", options)

```

###  Guarda anche
* modulo [aspose.cells.rendering](..)
