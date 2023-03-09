---
title: Metered класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 1050
url: /ru/python-net/aspose.cells/metered/
is_root: false
---
##  Metered класс
Предоставляет методы для установки измеренных клавиш.



Тип Metered предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [Metered()](/cells/ru/python-net/aspose.cells/metered/__init__/#) | Инициализирует новый экземпляр этого класса.|


###  Методы
| Метод| Описание|
| :- | :- |
| [set_metered_key(public_key, private_key)](/cells/ru/python-net/aspose.cells/metered/set_metered_key/#str-str) | Устанавливает дозированные открытые и закрытые ключи.<br/>Если вы покупаете ограниченную лицензию, при запуске приложения следует звонить по этому номеру API, обычно этого достаточно, вы должны регулярно проверять статус лицензии, если это статус оценки, звоните по этому номеру API снова.|
| [get_consumption_quantity()](/cells/ru/python-net/aspose.cells/metered/get_consumption_quantity/#) | Получает размер файла потребления|
| [get_consumption_credit()](/cells/ru/python-net/aspose.cells/metered/get_consumption_credit/#) | Получает потребительский кредит|



###  Примеры

В этом примере будет предпринята попытка установить лимитированные открытый и закрытый ключи.


```python
from aspose.cells import Metered

matered = Metered()
matered.set_metered_key("PublicKey", "PrivateKey")

```

###  Смотрите также
* модуль [aspose.cells](..)
