---
title: "Validation.ClientValidationFunction"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Validation. Получает или задает имя клиентской функции JavaScript проверки"
type: docs
url: /ru/net/aspose.cells.gridweb/validation/clientvalidationfunction/
---
## Validation.ClientValidationFunction property

Получает или задает имя JavaScript функции клиентской проверки.

```csharp
public string ClientValidationFunction { get; set; }
```

### Примечания

Используйте свойство ClientValidationFunction, чтобы указать имя клиентской функции проверки. Функция должна быть объявлена в следующей форме: `function customValicationFunction(source, value)` Параметр "source" — объект ячейки. Параметр "value" — строковое значение ячейки, которое нужно проверить. Функция должна возвращать true, если значение корректно.

### См. также

* class [Validation](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


