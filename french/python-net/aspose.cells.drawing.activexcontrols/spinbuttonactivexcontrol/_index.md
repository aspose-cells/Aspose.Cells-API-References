---
title: SpinButtonActiveXControl classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 110
url: /fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/
is_root: false
---
##  SpinButtonActiveXControl classe
Représente le contrôle SpinButton.



**Héritage:** [SpinButtonActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol) → 
[ActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrol) → 
[ActiveXControlBase](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)



Le type SpinButtonActiveXControl expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [workbook](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/workbook) | Obtient l'objet [ActiveXControlBase.workbook](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase#workbook).|
| [type](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/type) | Obtient le type du contrôle ActiveX.|
| [width](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/width) |Obtient et définit la largeur du contrôle en unité de points.|
| [height](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/height) | Obtient et définit la hauteur du contrôle en unités de points.|
| [mouse_icon](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/mouse_icon) | Obtient et définit une icône personnalisée à afficher comme pointeur de souris pour le contrôle.|
| [mouse_pointer](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/mouse_pointer) | Obtient et définit le type d'icône affichée comme pointeur de souris pour le contrôle.|
| [fore_ole_color](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/fore_ole_color) | Obtient et définit l'ancienne couleur du premier plan.|
| [back_ole_color](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/back_ole_color) | Obtient et définit l'ancienne couleur de l'arrière-plan.|
| [is_visible](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_visible) | Indique si ce contrôle est visible.|
| [shadow](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/shadow) | Indique s'il faut afficher une ombre.|
| [linked_cell](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/linked_cell) | Obtient et définit la cellule liée.|
| [list_fill_range](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/list_fill_range) | Obtient et définit la plage de remplissage de la liste.|
| [data](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/data) | Obtient et définit les données binaires du contrôle.|
| [is_enabled](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_enabled) | Indique si le contrôle peut recevoir le focus et répondre aux événements générés par l'utilisateur.|
| [is_locked](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_locked) | Indique si les données du contrôle sont verrouillées pour modification.|
| [is_transparent](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_transparent) | Indique si le champ est transparent.|
| [is_auto_size](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_auto_size) | Indique si le contrôle se redimensionne automatiquement pour afficher tout son contenu.|
| [ime_mode](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/ime_mode) |Obtient et définit le mode d'exécution par défaut de l'éditeur de méthode d'entrée pour le contrôle lorsqu'il reçoit le focus.|
| [font](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/font) | Représente la police du contrôle.|
| [text_align](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/text_align) | Représente comment aligner le texte utilisé par le contrôle.|
| [min](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/min) | Obtient et définit la valeur minimale acceptable.|
| [max](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/max) | Obtient et définit la valeur maximale acceptable.|
| [position](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/position) | Obtient et définit la valeur.|
| [small_change](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/small_change) | Obtient et définit la quantité de modification de la propriété Position|
| [orientation](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/orientation) | Obtient et définit si SpinButton ou ScrollBar est orienté verticalement ou horizontalement.|



###  Exemple

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

###  Voir également
* module [aspose.cells.drawing.activexcontrols](..)
* classe [ActiveXControl](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
* classe [ActiveXControlBase](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)
* classe [SpinButtonActiveXControl](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol)
