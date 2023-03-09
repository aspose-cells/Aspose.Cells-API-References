---
title: classe Style
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 1390
url: /it/python-net/aspose.cells/style/
is_root: false
---
##  classe Style
Rappresenta lo stile di visualizzazione del documento Excel, come carattere, colore, allineamento, bordo, ecc.
L'oggetto Style contiene tutti gli attributi di stile (carattere, formato numerico, allineamento e così via) come proprietà.



Il tipo Style espone i membri seguenti:

###  Costruttori
| Costruttore| Descrizione|
| :- | :- |
| [Style()](/cells/it/python-net/aspose.cells/style/__init__/#) | Inizializza una nuova istanza della classe [Style](/cells/it/python-net/aspose.cells/style).|


###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [background_theme_color](/cells/it/python-net/aspose.cells/style/background_theme_color) | Ottiene e imposta il colore del tema di sfondo.|
| [foreground_theme_color](/cells/it/python-net/aspose.cells/style/foreground_theme_color) | Ottiene e imposta il colore del tema in primo piano.|
| [name](/cells/it/python-net/aspose.cells/style/name) | Ottiene o imposta il nome dello stile.|
| [pattern](/cells/it/python-net/aspose.cells/style/pattern) |Ottiene o imposta il tipo di motivo di sfondo della cella.|
| [borders](/cells/it/python-net/aspose.cells/style/borders) | Ottiene lo [BorderCollection](/cells/it/python-net/aspose.cells/bordercollection) dello stile.|
| [background_color](/cells/it/python-net/aspose.cells/style/background_color) | Ottiene o imposta il colore di sfondo di uno stile.|
| [background_argb_color](/cells/it/python-net/aspose.cells/style/background_argb_color) | Ottiene e imposta il colore di sfondo con un valore ARGB a 32 bit.|
| [foreground_color](/cells/it/python-net/aspose.cells/style/foreground_color) | Ottiene o imposta il colore di primo piano di uno stile.|
| [foreground_argb_color](/cells/it/python-net/aspose.cells/style/foreground_argb_color) | Ottiene e imposta il colore di primo piano con un valore ARGB a 32 bit.|
| [has_borders](/cells/it/python-net/aspose.cells/style/has_borders) | Controlla se sono stati impostati bordi per lo stile.|
| [parent_style](/cells/it/python-net/aspose.cells/style/parent_style) | Ottiene lo stile padre di questo stile.|
| [indent_level](/cells/it/python-net/aspose.cells/style/indent_level) | Rappresenta il livello di rientro per la cella o l'intervallo.|
| [font](/cells/it/python-net/aspose.cells/style/font) | Ottiene un oggetto [Style.font](/cells/it/python-net/aspose.cells/style#font).|
| [rotation_angle](/cells/it/python-net/aspose.cells/style/rotation_angle) | Rappresenta l'angolo di rotazione del testo.|
| [horizontal_alignment](/cells/it/python-net/aspose.cells/style/horizontal_alignment) | Ottiene o imposta il tipo di allineamento orizzontale del testo in una cella.|
| [vertical_alignment](/cells/it/python-net/aspose.cells/style/vertical_alignment) | Ottiene o imposta il tipo di allineamento verticale del testo in una cella.|
| [is_text_wrapped](/cells/it/python-net/aspose.cells/style/is_text_wrapped) | Ottiene o imposta un valore che indica se il testo all'interno di una cella è a capo.|
| [number](/cells/it/python-net/aspose.cells/style/number) | Ottiene o imposta il formato di visualizzazione di numeri e date.|
| [is_locked](/cells/it/python-net/aspose.cells/style/is_locked) |Ottiene o imposta un valore che indica se una cella può essere modificata o meno.|
| [custom](/cells/it/python-net/aspose.cells/style/custom) | Rappresenta la stringa di formato numerico personalizzata di questo oggetto di stile.<br/> Se il formato numerico personalizzato non è impostato (ad esempio, il formato numerico è incorporato), verrà restituito "".|
| [culture_custom](/cells/it/python-net/aspose.cells/style/culture_custom) | Ottiene e imposta la stringa del modello dipendente dalle impostazioni cultura per il formato numerico.<br/>Se non è stato impostato alcun formato numerico per questo oggetto, verrà restituito null.<br/> Se il formato del numero è incorporato, verrà restituita la stringa del modello corrispondente al numero incorporato.|
| [invariant_custom](/cells/it/python-net/aspose.cells/style/invariant_custom) | Ottiene la stringa del modello indipendente dalle impostazioni cultura per il formato numerico.<br/>Se non è stato impostato alcun formato numerico per questo oggetto, verrà restituito null.<br/> Se il formato del numero è incorporato, verrà restituita la stringa del modello corrispondente al numero incorporato.|
| [is_formula_hidden](/cells/it/python-net/aspose.cells/style/is_formula_hidden) | Indica se la formula sarà nascosta quando il foglio di lavoro è protetto.|
| [shrink_to_fit](/cells/it/python-net/aspose.cells/style/shrink_to_fit) | Indica se il testo si riduce automaticamente per adattarsi alla larghezza della colonna disponibile.|
| [text_direction](/cells/it/python-net/aspose.cells/style/text_direction) | Rappresenta l'ordine di lettura del testo.|
| [is_justify_distributed](/cells/it/python-net/aspose.cells/style/is_justify_distributed) | Indica se l'allineamento giustificato o distribuito delle celle deve essere utilizzato sull'ultima riga di testo.|
| [quote_prefix](/cells/it/python-net/aspose.cells/style/quote_prefix) | Indica se il valore della cella inizia con una singola virgoletta.|
| [is_gradient](/cells/it/python-net/aspose.cells/style/is_gradient) | Indica se l'ombreggiatura della cella è un motivo sfumato.|
| [is_percent](/cells/it/python-net/aspose.cells/style/is_percent) |Indica se il formato numerico è un formato percentuale.|
| [is_date_time](/cells/it/python-net/aspose.cells/style/is_date_time) | Indica se il formato numerico è un formato data.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [set_border(border_type, border_style, border_color)](/cells/it/python-net/aspose.cells/style/set_border/#BorderType-CellBorderType-aspose.pydrawing.Color) | Imposta i bordi dello stile.|
| [set_border(border_type, border_style, border_color)](/cells/it/python-net/aspose.cells/style/set_border/#BorderType-CellBorderType-CellsColor) | Imposta i bordi dello stile.|
| [set_pattern_color(pattern, color1, color2)](/cells/it/python-net/aspose.cells/style/set_pattern_color/#BackgroundType-aspose.pydrawing.Color-aspose.pydrawing.Color) | Imposta il colore di sfondo.|
| [copy(style)](/cells/it/python-net/aspose.cells/style/copy/#Style) | Copia i dati da un altro oggetto di stile|
| [update()](/cells/it/python-net/aspose.cells/style/update/#) | Applica lo stile con nome agli stili delle celle che utilizzano questo stile con nome.<br/>Funziona come fare clic sul pulsante "ok" dopo aver finito di modificare lo stile.<br/> Si applica solo allo stile con nome.|
| [is_modified(modify_flag)](/cells/it/python-net/aspose.cells/style/is_modified/#StyleModifyFlag) | Controlla se le proprietà specificate dello stile sono state modificate.<br/> Utilizzato per lo stile di ConditionalFormattings per verificare se le proprietà specificate di questo stile devono essere utilizzate quando si applicano ConditionalFormattings a una cella.|
| [set_custom(custom, builtin_preference)](/cells/it/python-net/aspose.cells/style/set_custom/#str-bool) | Imposta la stringa di formato numero personalizzato di una cella.|
| [set_two_color_gradient(color1, color2, gradient_style_type, variant)](/cells/it/python-net/aspose.cells/style/set_two_color_gradient/#aspose.pydrawing.Color-aspose.pydrawing.Color-aspose.cells.drawing.GradientStyleType-int) | Imposta il riempimento specificato su una sfumatura a due colori.|
| [get_two_color_gradient(color1, color2, gradient_style_type, variant)](/cells/it/python-net/aspose.cells/style/get_two_color_gradient/#aspose.pydrawing.Color&-aspose.pydrawing.Color&-any-any) | Ottieni l'impostazione del gradiente a due colori.|
| [get_two_color_gradient_setting()](/cells/it/python-net/aspose.cells/style/get_two_color_gradient_setting/#) | Ottieni l'impostazione del gradiente a due colori.|
| [to_json()](/cells/it/python-net/aspose.cells/style/to_json/#) | Converti i dati struct [Style](/cells/it/python-net/aspose.cells/style) in JSON.|



###  Esempi

```python
from aspose.cells import Workbook
from aspose.pydrawing import Color

workbook = Workbook()
sheets = workbook.worksheets
cell = sheets[0].cells.get("A1")
style = cell.get_style()
style.font.name = "Times New Roman"
style.font.color = Color.blue
cell.set_style(style)

```

###  Guarda anche
* modulo [aspose.cells](..)
* classe [BorderCollection](/cells/it/python-net/aspose.cells/bordercollection)
* classe [Style](/cells/it/python-net/aspose.cells/style)
