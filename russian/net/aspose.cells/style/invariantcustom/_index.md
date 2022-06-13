---
title: InvariantCustom
second_title: Справочник по Aspose.Cells для .NET API
description: Получает строку шаблона не зависящую от языка и региональных параметров для числового формата. Если для этого объекта не задан числовой формат будет возвращено значение null. Если числовой формат является встроенным будет возвращена строка шаблона соответствующая встроенному числу.
type: docs
weight: 140
url: /ru/net/aspose.cells/style/invariantcustom/
---
## Style.InvariantCustom property

Получает строку шаблона, не зависящую от языка и региональных параметров, для числового формата. Если для этого объекта не задан числовой формат, будет возвращено значение null. Если числовой формат является встроенным, будет возвращена строка шаблона, соответствующая встроенному числу.

```csharp
public string InvariantCustom { get; }
```

### Примечания

Для встроенных числовых форматов возвращаемое содержимое шаблона по-прежнему зависит от языка и региональных параметров, например, для некоторых локалей он возвращает "m/d/y", а для некоторых других локалей возвращает "d/m/y". Отличие от[`CultureCustom`](../culturecustom)в том, что (это также означает независимость от культуры): спецификаторы формата и разделители остаются стандартными, например, '/' всегда будет использоваться в качестве разделителя даты и времени , а "y" всегда будет использоваться в качестве части "год", независимо от того, какой другой специальный символ используется для конкретного локаль.

### Смотрите также

* class [Style](../../style)
* пространство имен [Aspose.Cells](../../style)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->