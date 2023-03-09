---
title: emf_render_setting propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 200
url: /es/python-net/aspose.cells/pdfsaveoptions/emf_render_setting/
is_root: false
---
##  emf_render_setting propiedad

Configuración para renderizar el metarchivo Emf.

###  Observaciones

 Los metarchivos EMF identificados como "EMF+ Dual" pueden contener registros EMF+ y registros EMF.
Se puede usar cualquier tipo de registro para representar la imagen, solo EMF+ registros o solo EMF registros.
Cuando se establece [EmfRenderSetting.EMF_PLUS_PREFER](/cells/es/python-net/aspose.cells/emfrendersetting#EMF_PLUS_PREFER), se analizarán EMF+ registros mientras se procesan en pdf; de lo contrario, solo se analizarán EMF registros.
El valor predeterminado es [EmfRenderSetting.EMF_ONLY](/cells/es/python-net/aspose.cells/emfrendersetting#EMF_ONLY).
###  Definición:
```python
@property
def emf_render_setting(self):
    ...
@emf_render_setting.setter
def emf_render_setting(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells](../../)
* clase [EmfRenderSetting](/cells/es/python-net/aspose.cells/emfrendersetting)
* clase [PdfSaveOptions](/cells/es/python-net/aspose.cells/pdfsaveoptions)
