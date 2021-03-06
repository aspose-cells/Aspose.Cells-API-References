---
title: CultureCustom
second_title: Справочник по Aspose.Cells для .NET API
description: Получает и задает строку шаблона зависящую от языка и региональных параметров для числового формата. Если для этого объекта не задан числовой формат будет возвращено значение null. Если числовой формат является встроенным будет возвращена строка шаблона соответствующая встроенному числу.
type: docs
weight: 50
url: /ru/net/aspose.cells/style/culturecustom/
---
## Style.CultureCustom property

Получает и задает строку шаблона, зависящую от языка и региональных параметров, для числового формата. Если для этого объекта не задан числовой формат, будет возвращено значение null. Если числовой формат является встроенным, будет возвращена строка шаблона, соответствующая встроенному числу.

```csharp
public string CultureCustom { get; set; }
```

### Примечания

Для встроенного числового формата содержимое шаблона (например, один встроенный формат даты "m /d/y" для некоторых локалей, но для некоторых других локалей становится "d/m/y") и спецификатор формата (например, некоторые локали используют символ, отличный от 'y' для представления части года для форматирования даты) зависят от региональных параметров; Для заданного пользователем пользовательского формата изменяются только спецификаторы формата в соответствии с культурой, другие части шаблона форматирования не будут изменены.

### Смотрите также

* class [Style](../../style)
* пространство имен [Aspose.Cells](../../style)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
