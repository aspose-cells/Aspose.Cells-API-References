---
title: "DocumentProperty.ToDouble"
second_title: "Справочник API Aspose.Cells для .NET"
description: "DocumentProperty method. Возвращает значение свойства как double"
type: docs
url: /ru/net/aspose.cells.properties/documentproperty/todouble/
---
## DocumentProperty.ToDouble method

Возвращает значение свойства как double.

```csharp
public double ToDouble()
```

### Примечания

Выбрасывает исключение, если тип свойства не PropertyType.Float.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToDoubleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получите коллекцию пользовательских свойств документа
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Добавьте числовое свойство
            customProperties.Add("Rating", 4.75);

            // Получите свойство и преобразуйте в double
            DocumentProperty ratingProperty = customProperties["Rating"];
            double ratingValue = ratingProperty.ToDouble();

            // Вывести результат.
            Console.WriteLine($"Rating: {ratingValue}");

            // Сохраните книгу
            workbook.Save("DocumentPropertyToDoubleExample.xlsx");
        }
    }
}
```

### См. также

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


