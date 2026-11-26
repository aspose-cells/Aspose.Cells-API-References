---
title: "DocumentProperty.ToDateTime"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод DocumentProperty. Возвращает значение свойства как DateTime в локальном часовом поясе"
type: docs
url: /ru/net/aspose.cells.properties/documentproperty/todatetime/
---
## DocumentProperty.ToDateTime method

Возвращает значение свойства как DateTime в локальном часовом поясе.

```csharp
public DateTime ToDateTime()
```

### Примечания

Выбрасывает исключение, если тип свойства не PropertyType.Date.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToDateTimeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получите коллекцию пользовательских свойств документа
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Добавьте свойство datetime
            DateTime currentTime = DateTime.Now;
            customProperties.Add("LastModified", currentTime);

            // Получите свойство и преобразуйте его в DateTime
            DocumentProperty lastModifiedProperty = customProperties["LastModified"];
            DateTime retrievedTime = lastModifiedProperty.ToDateTime();

            // Вывести результат.
            Console.WriteLine($"Stored DateTime: {currentTime}");
            Console.WriteLine($"Retrieved DateTime: {retrievedTime}");

            // Сохраните книгу
            workbook.Save("DocumentPropertyDateTimeExample.xlsx");
        }
    }
}
```

### См. также

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


