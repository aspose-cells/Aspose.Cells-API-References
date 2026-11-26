---
title: "GridValidation.ClientValidationFunction"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство GridValidation. Возвращает или задает имя клиентской функции проверки JavaScript"
type: docs
url: /ru/net/aspose.cells.griddesktop.data/gridvalidation/clientvalidationfunction/
---
## GridValidation.ClientValidationFunction property

Получает или задает имя JavaScript функции клиентской проверки.

```csharp
public string ClientValidationFunction { get; set; }
```

### Примечания

Используйте свойство ClientValidationFunction, чтобы указать имя клиентской функции проверки. Функция должна быть объявлена в следующей форме: `function customValicationFunction(source, value)` Параметр "source" — объект ячейки. Параметр "value" — строковое значение ячейки, которое нужно проверить. Функция должна возвращать true, если значение корректно.

### См. также

* class [GridValidation](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


