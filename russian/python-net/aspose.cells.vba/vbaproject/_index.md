---
title: VbaProject класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 30
url: /ru/python-net/aspose.cells.vba/vbaproject/
is_root: false
---
##  VbaProject класс
Представляет проект VBA.



Тип VbaProject предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [is_valid_signed](/cells/ru/python-net/aspose.cells.vba/vbaproject/is_valid_signed) | Указывает, действительна ли подпись проекта VBA.|
| [cert_raw_data](/cells/ru/python-net/aspose.cells.vba/vbaproject/cert_raw_data) | Получает необработанные данные сертификата, если этот проект VBA подписан.|
| [name](/cells/ru/python-net/aspose.cells.vba/vbaproject/name) | Получает и задает имя проекта VBA.|
| [is_signed](/cells/ru/python-net/aspose.cells.vba/vbaproject/is_signed) | Указывает, подписан VBAcode или нет.|
| [is_protected](/cells/ru/python-net/aspose.cells.vba/vbaproject/is_protected) | Указывает, защищен ли этот проект VBA.|
| [islocked_for_viewing](/cells/ru/python-net/aspose.cells.vba/vbaproject/islocked_for_viewing) | Указывает, заблокирован ли этот проект VBA для просмотра.|
| [modules](/cells/ru/python-net/aspose.cells.vba/vbaproject/modules) | Получает все [VbaModule](/cells/ru/python-net/aspose.cells.vba/vbamodule) объектов.|
| [references](/cells/ru/python-net/aspose.cells.vba/vbaproject/references) | Получает все ссылки проекта VBA.|


###  Методы
| Метод| Описание|
| :- | :- |
| [sign(digital_signature)](/cells/ru/python-net/aspose.cells.vba/vbaproject/sign/#aspose.cells.digitalsignatures.DigitalSignature) | Подпишите этот проект VBA с помощью DigitalSignature|
| [protect(islocked_for_viewing, password)](/cells/ru/python-net/aspose.cells.vba/vbaproject/protect/#bool-str) | Защищает или снимает защиту с этого проекта VBA.|
| [copy(source)](/cells/ru/python-net/aspose.cells.vba/vbaproject/copy/#VbaProject) | Скопируйте проект VBA из другого файла.|
| [validate_password(password)](/cells/ru/python-net/aspose.cells.vba/vbaproject/validate_password/#str) | Проверяет пароль защиты.|



###  Пример

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
# Saving the Excel file
workbook.save("book1.xlsm")

```

###  Смотрите также
* модуль [aspose.cells.vba](..)
* класс [VbaModule](/cells/ru/python-net/aspose.cells.vba/vbamodule)
