---
title: emf_render_setting proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 200
url: /it/python-net/aspose.cells/pdfsaveoptions/emf_render_setting/
is_root: false
---
##  emf_render_setting proprietà

Impostazione per il rendering del metafile EMF.

###  Osservazioni

 I metafile EMF identificati come "EMF+ Dual" possono contenere sia record EMF+ sia record EMF.
Entrambi i tipi di record possono essere utilizzati per il rendering dell'immagine, solo record EMF+ o solo record EMF.
Quando è impostato [EmfRenderSetting.EMF_PLUS_PREFER](/cells/it/python-net/aspose.cells/emfrendersetting#EMF_PLUS_PREFER), verranno analizzati EMF+ record durante il rendering in pdf, altrimenti verranno analizzati solo i record EMF.
Il valore predefinito è [EmfRenderSetting.EMF_ONLY](/cells/it/python-net/aspose.cells/emfrendersetting#EMF_ONLY).
###  Definizione:
```python
@property
def emf_render_setting(self):
    ...
@emf_render_setting.setter
def emf_render_setting(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells](../../)
* classe [EmfRenderSetting](/cells/it/python-net/aspose.cells/emfrendersetting)
* classe [PdfSaveOptions](/cells/it/python-net/aspose.cells/pdfsaveoptions)
