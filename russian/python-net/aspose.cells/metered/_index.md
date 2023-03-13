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
Предоставляет методы для установки измеренного ключа.



Тип Metered предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [Metered()](/cells/ru/python-net/aspose.cells/metered/__init__/#) | Инициализирует новый экземпляр этого класса.|


###  Методы
| Метод| Описание|
| :- | :- |
| [set_metered_key(public_key, private_key)](/cells/ru/python-net/aspose.cells/metered/set_metered_key/#str-str) | Устанавливает измеренный открытый и закрытый ключ.<br/>Если вы покупаете лимитную лицензию, при запуске приложения следует позвонить по этому номеру API, обычно этого достаточно. Однако, если всегда не удается загрузить данные о потреблении и время превышает 24 часа, лицензия будет установлена в ознакомительный статус, чтобы избежать этого, вы должны регулярно проверять статус лицензии, если это ознакомительный статус, снова звоните по этому номеру API.|
| [get_consumption_quantity()](/cells/ru/python-net/aspose.cells/metered/get_consumption_quantity/#) | Получает размер файла потребления|
| [get_consumption_credit()](/cells/ru/python-net/aspose.cells/metered/get_consumption_credit/#) | Получает потребительский кредит|



###  Пример

В этом примере будет предпринята попытка установить лимитный открытый и закрытый ключ.


```python
from aspose.cells import Metered

matered = Metered()
matered.set_metered_key("PublicKey", "PrivateKey")

```

###  Смотрите также
* модуль [aspose.cells](..)
