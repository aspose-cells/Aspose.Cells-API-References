---
title: SignatureLine класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 640
url: /ru/python-net/aspose.cells.drawing/signatureline/
is_root: false
---
##  SignatureLine класс
Представляют строку подписи.



Тип SignatureLine предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [SignatureLine()](/cells/ru/python-net/aspose.cells.drawing/signatureline/__init__/#) | Создает новый экземпляр SignatureLine|


###  Характеристики
| Свойство| Описание|
| :- | :- |
| [id](/cells/ru/python-net/aspose.cells.drawing/signatureline/id) | Получает или задает идентификатор для этой строки подписи.|
| [provider_id](/cells/ru/python-net/aspose.cells.drawing/signatureline/provider_id) | Получает и задает идентификатор поставщика подписи.|
| [signer](/cells/ru/python-net/aspose.cells.drawing/signatureline/signer) | Получает и задает подписывающую сторону.|
| [title](/cells/ru/python-net/aspose.cells.drawing/signatureline/title) | Получает и устанавливает звание певицы.|
| [email](/cells/ru/python-net/aspose.cells.drawing/signatureline/email) | Получает и устанавливает адрес электронной почты певца.|
| [is_line](/cells/ru/python-net/aspose.cells.drawing/signatureline/is_line) | Указывает, является ли это строкой подписи.|
| [allow_comments](/cells/ru/python-net/aspose.cells.drawing/signatureline/allow_comments) | Указывает, можно ли прикреплять комментарии.|
| [show_signed_date](/cells/ru/python-net/aspose.cells.drawing/signatureline/show_signed_date) | Указывает, показывать ли подписанную дату.|
| [instructions](/cells/ru/python-net/aspose.cells.drawing/signatureline/instructions) | Получает и задает текст, отображаемый пользователю во время подписания.|



###  Пример

```python
from aspose.cells import Workbook
from aspose.cells.drawing import SignatureLine

# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
# Adding a picture
imgIndex = worksheet.pictures.add(1, 1, "sample.png")
pic = worksheet.pictures[imgIndex]
#  Create signature line object
s = SignatureLine()
s.signer = "Simon Zhao"
s.title = "Development Lead"
s.email = "Simon.Zhao@aspose.com"
#  Assign the signature line object to Picture.SignatureLine property
pic.signature_line = s
# do your business
# Save the excel file.
workbook.save("result.xlsx")

```

###  Смотрите также
* модуль [aspose.cells.drawing](..)
