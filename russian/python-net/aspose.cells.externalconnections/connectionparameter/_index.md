---
title: ConnectionParameter класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 10
url: /ru/python-net/aspose.cells.externalconnections/connectionparameter/
is_root: false
---
##  ConnectionParameter класс
Указывает свойства любых параметров, используемых с внешними подключениями к данным.
Параметры действительны для ODBC и веб-запросов.



Тип ConnectionParameter предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [sql_type](/cells/ru/python-net/aspose.cells.externalconnections/connectionparameter/sql_type) | Тип данных SQL параметра. Допустимо только для источников ODBC.|
| [refresh_on_change](/cells/ru/python-net/aspose.cells.externalconnections/connectionparameter/refresh_on_change) | Флаг, указывающий, должен ли запрос автоматически обновляться, когда содержимое<br/> ячейка, которая обеспечивает изменение значения параметра. Если true, то внешние данные обновляются<br/> используя новое значение параметра каждый раз при изменении. Если false, то внешние данные<br/> обновляется только по запросу пользователя, или какое-либо другое событие запускает обновление (например, открытие рабочей книги).|
| [prompt](/cells/ru/python-net/aspose.cells.externalconnections/connectionparameter/prompt) | Строка подсказки для параметра. Предоставляется пользователю электронной таблицы вместе с пользовательским интерфейсом ввода.<br/> для сбора значения параметра перед обновлением внешних данных. Используется только тогда, когда<br/>тип параметра = подсказка.|
| [type](/cells/ru/python-net/aspose.cells.externalconnections/connectionparameter/type) | Тип используемого параметра.<br/> Если параметрType=value, то значение из логического, двойного, целого,<br/> или строка будет использоваться. В этом случае ожидается, что только один из<br/> {boolean, double, integer или string} будет указано.|
| [name](/cells/ru/python-net/aspose.cells.externalconnections/connectionparameter/name) | Имя параметра.|
| [cell_reference](/cells/ru/python-net/aspose.cells.externalconnections/connectionparameter/cell_reference) | Ссылка Cell, указывающая, какое значение ячейки использовать для параметра запроса. Используется только в том случае, если параметрType — это ячейка.|
| [value](/cells/ru/python-net/aspose.cells.externalconnections/connectionparameter/value) | Нецелое числовое значение, целочисленное значение, строковое значение или логическое значение<br/> для использования в качестве параметра запроса. Используется, только если параметрType имеет значение.|



###  Смотрите также
* модуль [aspose.cells.externalconnections](..)
