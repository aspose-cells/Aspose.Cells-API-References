---
title: emf_render_setting недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 200
url: /ru/python-net/aspose.cells/pdfsaveoptions/emf_render_setting/
is_root: false
---
##  emf_render_setting недвижимость

Настройка для рендеринга метафайла EMF.

###  Примечания

 Метафайлы EMF, обозначенные как «EMF+ Dual», могут содержать как записи EMF+, так и записи EMF.
Для рендеринга изображения можно использовать записи любого типа, только EMF+ записей или только EMF записей.
Если установлено значение [EmfRenderSetting.EMF_PLUS_PREFER](/cells/ru/python-net/aspose.cells/emfrendersetting#EMF_PLUS_PREFER), то при рендеринге в pdf будет проанализировано более EMF записей, в противном случае будет проанализировано только EMF записей.
Значение по умолчанию — [EmfRenderSetting.EMF_ONLY](/cells/ru/python-net/aspose.cells/emfrendersetting#EMF_ONLY).
###  Определение:
```python
@property
def emf_render_setting(self):
    ...
@emf_render_setting.setter
def emf_render_setting(self, value):
    ...
```

###  Смотрите также
* модуль [aspose.cells](../../)
* класс [EmfRenderSetting](/cells/ru/python-net/aspose.cells/emfrendersetting)
* класс [PdfSaveOptions](/cells/ru/python-net/aspose.cells/pdfsaveoptions)
