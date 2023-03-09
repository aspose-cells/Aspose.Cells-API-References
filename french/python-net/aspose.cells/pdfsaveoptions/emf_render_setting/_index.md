---
title: emf_render_setting propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 200
url: /fr/python-net/aspose.cells/pdfsaveoptions/emf_render_setting/
is_root: false
---
##  emf_render_setting propriété

Paramètre pour le rendu du métafichier Emf.

###  Remarques

 Les métafichiers EMF identifiés comme "EMF+ Dual" peuvent contenir à la fois des enregistrements EMF+ et des enregistrements EMF.
L'un ou l'autre type d'enregistrement peut être utilisé pour rendre l'image, uniquement les enregistrements EMF+ ou uniquement les enregistrements EMF.
Lorsque [EmfRenderSetting.EMF_PLUS_PREFER](/cells/fr/python-net/aspose.cells/emfrendersetting#EMF_PLUS_PREFER) est défini, les enregistrements EMF+ seront analysés lors du rendu en pdf, sinon seuls les enregistrements EMF seront analysés.
La valeur par défaut est [EmfRenderSetting.EMF_ONLY](/cells/fr/python-net/aspose.cells/emfrendersetting#EMF_ONLY).
###  Définition:
```python
@property
def emf_render_setting(self):
    ...
@emf_render_setting.setter
def emf_render_setting(self, value):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [EmfRenderSetting](/cells/fr/python-net/aspose.cells/emfrendersetting)
* classe [PdfSaveOptions](/cells/fr/python-net/aspose.cells/pdfsaveoptions)
