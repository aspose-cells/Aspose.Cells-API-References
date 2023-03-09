---
title: ToggleButtonActiveXControl classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 130
url: /fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/
is_root: false
---
##  ToggleButtonActiveXControl classe
Représente un contrôle ActiveX ToggleButton.



**Héritage:** [ToggleButtonActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol) → 
[ActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrol) → 
[ActiveXControlBase](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)



Le type ToggleButtonActiveXControl expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [workbook](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/workbook) | Obtient l'objet [ActiveXControlBase.workbook](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase#workbook).|
| [type](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/type) | Obtient le type du contrôle ActiveX.|
| [width](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/width) | Obtient et définit la largeur du contrôle en unités de points.|
| [height](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/height) | Obtient et définit la hauteur du contrôle en unités de points.|
| [mouse_icon](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/mouse_icon) | Obtient et définit une icône personnalisée à afficher comme pointeur de souris pour le contrôle.|
| [mouse_pointer](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/mouse_pointer) |Obtient et définit le type d'icône affichée comme pointeur de souris pour le contrôle.|
| [fore_ole_color](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/fore_ole_color) | Obtient et définit l'ancienne couleur du premier plan.|
| [back_ole_color](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/back_ole_color) | Obtient et définit l'ancienne couleur de l'arrière-plan.|
| [is_visible](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_visible) | Indique si ce contrôle est visible.|
| [shadow](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/shadow) | Indique s'il faut afficher une ombre.|
| [linked_cell](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/linked_cell) | Obtient et définit la cellule liée.|
| [list_fill_range](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/list_fill_range) | Obtient et définit la plage de remplissage de la liste.|
| [data](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/data) | Obtient et définit les données binaires du contrôle.|
| [is_enabled](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_enabled) | Indique si le contrôle peut recevoir le focus et répondre aux événements générés par l'utilisateur.|
| [is_locked](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_locked) | Indique si les données du contrôle sont verrouillées pour modification.|
| [is_transparent](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_transparent) |Indique si le champ est transparent.|
| [is_auto_size](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_auto_size) | Indique si le contrôle se redimensionne automatiquement pour afficher tout son contenu.|
| [ime_mode](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/ime_mode) | Obtient et définit le mode d'exécution par défaut de l'éditeur de méthode d'entrée pour le contrôle lorsqu'il reçoit le focus.|
| [font](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/font) | Représente la police du contrôle.|
| [text_align](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/text_align) | Représente comment aligner le texte utilisé par le contrôle.|
| [caption](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/caption) | Obtient et définit le texte descriptif qui apparaît sur un contrôle.|
| [picture_position](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/picture_position) | Obtient et définit l'emplacement de l'image du contrôle par rapport à sa légende.|
| [special_effect](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/special_effect) | Obtient et définit l'effet spécial du contrôle.|
| [picture](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/picture) |Obtient et définit les données de l'image.|
| [accelerator](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/accelerator) | Obtient et définit la touche de raccourci pour le contrôle.|
| [value](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/value) | Indique si le champ est coché ou non.|
| [is_triple_state](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_triple_state) | Indique comment le contrôle spécifié affichera les valeurs Null.|



###  Exemple

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

###  Voir également
* module [aspose.cells.drawing.activexcontrols](..)
* classe [ActiveXControl](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
* classe [ActiveXControlBase](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)
* classe [ToggleButtonActiveXControl](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol)
