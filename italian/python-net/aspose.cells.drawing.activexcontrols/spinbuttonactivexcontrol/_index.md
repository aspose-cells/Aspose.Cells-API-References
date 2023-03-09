---
title: classe SpinButtonActiveXControl
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 110
url: /it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/
is_root: false
---
##  classe SpinButtonActiveXControl
Rappresenta il controllo SpinButton.



**Eredità:** [SpinButtonActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol) → 
[ActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrol) → 
[ActiveXControlBase](/cells/it/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)



Il tipo SpinButtonActiveXControl espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [workbook](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/workbook) | Ottiene l'oggetto [ActiveXControlBase.workbook](/cells/it/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase#workbook).|
| [type](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/type) | Ottiene il tipo del controllo ActiveX.|
| [width](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/width) |Ottiene e imposta la larghezza del controllo in unità di punti.|
| [height](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/height) | Ottiene e imposta l'altezza del controllo in unità di punti.|
| [mouse_icon](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/mouse_icon) | Ottiene e imposta un'icona personalizzata da visualizzare come puntatore del mouse per il controllo.|
| [mouse_pointer](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/mouse_pointer) | Ottiene e imposta il tipo di icona visualizzata come puntatore del mouse per il controllo.|
| [fore_ole_color](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/fore_ole_color) | Ottiene e imposta il colore ole del primo piano.|
| [back_ole_color](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/back_ole_color) | Ottiene e imposta il colore ole dello sfondo.|
| [is_visible](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_visible) | Indica se questo controllo è visibile.|
| [shadow](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/shadow) | Indica se mostrare un'ombra.|
| [linked_cell](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/linked_cell) | Ottiene e imposta la cella collegata.|
| [list_fill_range](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/list_fill_range) | Ottiene e imposta l'intervallo di riempimento dell'elenco.|
| [data](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/data) | Ottiene e imposta i dati binari del controllo.|
| [is_enabled](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_enabled) | Indica se il controllo può ricevere lo stato attivo e rispondere agli eventi generati dall'utente.|
| [is_locked](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_locked) | Indica se i dati nel controllo sono bloccati per la modifica.|
| [is_transparent](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_transparent) | Indica se il controllo è trasparente.|
| [is_auto_size](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_auto_size) | Indica se il controllo verrà ridimensionato automaticamente per visualizzarne l'intero contenuto.|
| [ime_mode](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/ime_mode) |Ottiene e imposta la modalità di runtime predefinita dell'Input Method Editor per il controllo quando riceve lo stato attivo.|
| [font](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/font) | Rappresenta il tipo di carattere del controllo.|
| [text_align](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/text_align) | Rappresenta come allineare il testo utilizzato dal controllo.|
| [min](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/min) | Ottiene e imposta il valore minimo accettabile.|
| [max](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/max) | Ottiene e imposta il valore massimo accettabile.|
| [position](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/position) | Ottiene e imposta il valore.|
| [small_change](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/small_change) | Ottiene e imposta l'entità della modifica della proprietà Position|
| [orientation](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/orientation) | Ottiene e imposta se SpinButton o ScrollBar è orientato verticalmente o orizzontalmente.|



###  Esempi

```python
from aspose import pycore
from aspose.cells import Workbook
from aspose.cells.drawing.activexcontrols import ControlType, SpinButtonActiveXControl

# Initialize a new workbook.
book = Workbook()
# Add a ToggleButtonActiveXControl.
shape = book.worksheets[0].shapes.add_active_x_control(ControlType.SPIN_BUTTON, 1, 0, 1, 0, 100, 50)
activeXControl = pycore.cast(SpinButtonActiveXControl, shape.active_x_control)
# do your business
# Save the excel file.
book.save("exmaple.xlsx")

```

###  Guarda anche
* modulo [aspose.cells.drawing.activexcontrols](..)
* classe [ActiveXControl](/cells/it/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
* classe [ActiveXControlBase](/cells/it/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)
* classe [SpinButtonActiveXControl](/cells/it/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol)
