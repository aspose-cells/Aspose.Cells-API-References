---
title: classe ToggleButtonActiveXControl
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 130
url: /it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/
is_root: false
---
##  classe ToggleButtonActiveXControl
Rappresenta un controllo ActiveX ToggleButton.



**Eredità:** [ToggleButtonActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol) → 
[ActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrol) → 
[ActiveXControlBase](/cells/it/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)



Il tipo ToggleButtonActiveXControl espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [workbook](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/workbook) | Ottiene l'oggetto [ActiveXControlBase.workbook](/cells/it/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase#workbook).|
| [type](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/type) | Ottiene il tipo del controllo ActiveX.|
| [width](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/width) |Ottiene e imposta la larghezza del controllo in unità di punti.|
| [height](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/height) | Ottiene e imposta l'altezza del controllo in unità di punti.|
| [mouse_icon](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/mouse_icon) | Ottiene e imposta un'icona personalizzata da visualizzare come puntatore del mouse per il controllo.|
| [mouse_pointer](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/mouse_pointer) | Ottiene e imposta il tipo di icona visualizzata come puntatore del mouse per il controllo.|
| [fore_ole_color](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/fore_ole_color) | Ottiene e imposta il colore ole del primo piano.|
| [back_ole_color](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/back_ole_color) | Ottiene e imposta il colore ole dello sfondo.|
| [is_visible](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_visible) | Indica se questo controllo è visibile.|
| [shadow](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/shadow) | Indica se mostrare un'ombra.|
| [linked_cell](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/linked_cell) | Ottiene e imposta la cella collegata.|
| [list_fill_range](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/list_fill_range) | Ottiene e imposta l'intervallo di riempimento dell'elenco.|
| [data](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/data) | Ottiene e imposta i dati binari del controllo.|
| [is_enabled](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_enabled) | Indica se il controllo può ricevere lo stato attivo e rispondere agli eventi generati dall'utente.|
| [is_locked](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_locked) | Indica se i dati nel controllo sono bloccati per la modifica.|
| [is_transparent](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_transparent) | Indica se il controllo è trasparente.|
| [is_auto_size](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_auto_size) | Indica se il controllo verrà ridimensionato automaticamente per visualizzarne l'intero contenuto.|
| [ime_mode](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/ime_mode) |Ottiene e imposta la modalità di runtime predefinita dell'Input Method Editor per il controllo quando riceve lo stato attivo.|
| [font](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/font) | Rappresenta il tipo di carattere del controllo.|
| [text_align](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/text_align) | Rappresenta come allineare il testo utilizzato dal controllo.|
| [caption](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/caption) | Ottiene e imposta il testo descrittivo visualizzato su un controllo.|
| [picture_position](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/picture_position) | Ottiene e imposta la posizione dell'immagine del controllo rispetto alla relativa didascalia.|
| [special_effect](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/special_effect) | Ottiene e imposta l'effetto speciale del controllo.|
| [picture](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/picture) | Ottiene e imposta i dati dell'immagine.|
| [accelerator](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/accelerator) | Ottiene e imposta il tasto di scelta rapida per il controllo.|
| [value](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/value) |Indica se il controllo è selezionato o meno.|
| [is_triple_state](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_triple_state) | Indica come il controllo specificato visualizzerà i valori Null.|



###  Esempio

```python
from aspose import pycore
from aspose.cells import Workbook
from aspose.cells.drawing.activexcontrols import ControlType, ToggleButtonActiveXControl

# Initialize a new workbook.
book = Workbook()
# Add a ToggleButtonActiveXControl.
shape = book.worksheets[0].shapes.add_active_x_control(ControlType.TOGGLE_BUTTON, 1, 0, 1, 0, 100, 50)
activeXControl = pycore.cast(ToggleButtonActiveXControl, shape.active_x_control)
# do your business
# Save the excel file.
book.save("exmaple.xlsx")

```

###  Guarda anche
* modulo [aspose.cells.drawing.activexcontrols](..)
* classe [ActiveXControl](/cells/it/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
* classe [ActiveXControlBase](/cells/it/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)
* classe [ToggleButtonActiveXControl](/cells/it/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol)
