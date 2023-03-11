---
title: set_embedded_object méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 170
url: /fr/python-net/aspose.cells.drawing/oleobject/set_embedded_object/
is_root: false
---
##  set_embedded_object(link_to_file, object_data, source_file_name, display_as_icon, label) {#bool-bytes-str-bool-str}
Définit les données d'objet incorporées.



```python
def set_embedded_object(self, link_to_file, object_data, source_file_name, display_as_icon, label):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| link_to_file | bool | Indique si l'objet est lié au fichier. Si vrai, le paramètre objectData est ignoré.|
| object_data | bytes | Les données d'objet incorporées.|
| source_file_name | str | Le nom du fichier.|
| display_as_icon | bool | Indique si l'objet est affiché sous forme d'icône.<br/> Si vrai, les données d'image d'origine seront couvertes par l'icône.|
| label | str | L'étiquette de l'icône. Ne fonctionne que lorsque displayAsIcon a la valeur true.|


##  set_embedded_object(link_to_file, object_data, source_file_name, display_as_icon, label, update_icon) {#bool-bytes-str-bool-str-bool}
Définit les données d'objet incorporées.



```python
def set_embedded_object(self, link_to_file, object_data, source_file_name, display_as_icon, label, update_icon):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| link_to_file | bool | Indique si l'objet est lié au fichier. Si vrai, le paramètre objectData est ignoré.|
| object_data | bytes | Les données d'objet incorporées.|
| source_file_name | str | Le nom du fichier.|
| display_as_icon | bool | Indique si l'objet est affiché sous forme d'icône.<br/> Si vrai, les données d'image d'origine seront couvertes par l'icône.|
| label | str | L'étiquette de l'icône. Ne fonctionne que lorsque displayAsIcon a la valeur true.|
| update_icon | bool | Indique si l'icône de mise à jour automatique.|
###  Remarques

Comme Aspose peut mettre à jour toutes les icônes de fichiers, il est donc préférable que vous puissiez ajouter l'icône correcte avec `update_icon` comme faux.


###  Voir également

* module [aspose.cells.drawing](../../)
* classe [OleObject](/cells/fr/python-net/aspose.cells.drawing/oleobject)
