---
title: is_param_literal_required недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 40
url: /ru/python-net/aspose.cells/abstractcalculationengine/is_param_literal_required/
is_root: false
---
##  is_param_literal_required недвижимость

Указывает, нужен ли этому движку литеральный текст параметра при выполнении расчета.Значение по умолчанию — false.

###  Примечания

Если для этого пользовательского механизма вычислений требуется литеральный текст параметра, потребуется больше стеков для кэширования литерального текста для параметров, и метод Calculate() может вызываться рекурсивно для вычисления значения параметра.
Обычно литеральный текст не требуется для вычисления формул, и этот метод должен возвращать false для большинства реализаций, чтобы повысить производительность.
###  Определение:
```python
@property
def is_param_literal_required(self):
    ...
```

###  Смотрите также
* модуль [aspose.cells](../../)
* класс [AbstractCalculationEngine](/cells/ru/python-net/aspose.cells/abstractcalculationengine)
