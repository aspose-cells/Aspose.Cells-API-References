---
title: DigitalSignatureCollection класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 20
url: /ru/python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/
is_root: false
---
##  DigitalSignatureCollection класс
Предоставляет набор цифровых подписей, прикрепленных к документу.



Тип DigitalSignatureCollection предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [DigitalSignatureCollection()](/cells/ru/python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/__init__/#) | Конструктор DigitalSignatureCollection.|


###  Методы
| Метод| Описание|
| :- | :- |
| [add(digital_signature)](/cells/ru/python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/add/#DigitalSignature) |Добавьте одну подпись в DigitalSignatureCollection.|



###  Пример

В следующем примере показано, как проверить цифровую подпись.

```python
from aspose.cells import Workbook

# workbook from a signed source file
signedWorkbook = Workbook(r"signedFile.xlsx")
# wb.IsDigitallySigned is true when the workbook is signed already.
print(signedWorkbook.is_digitally_signed)
# get digitalSignature collection from workbook
existingDsc = signedWorkbook.get_digital_signature()
for existingDs in existingDsc:
    print(existingDs.comments)
    print(existingDs.sign_time)
    print(existingDs.is_valid)

```

###  Смотрите также
* модуль [aspose.cells.digitalsignatures](..)
