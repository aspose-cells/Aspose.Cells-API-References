---
title: "DocumentProperty.ToInt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод DocumentProperty. Возвращает значение свойства как целое число"
type: docs
url: /ru/net/aspose.cells.properties/documentproperty/toint/
---
## DocumentProperty.ToInt method

Возвращает значение свойства как integer.

```csharp
public int ToInt()
```

### Примечания

Выбрасывает исключение, если тип свойства не PropertyType.Number.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToIntDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить коллекцию пользовательских свойств документа
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Добавить числовое пользовательское свойство
            customProperties.Add("Revision", 5);

            // Получите свойство и преобразуйте его в int, используя ToInt()
            DocumentProperty revisionProperty = customProperties["Revision"];
            int revisionValue = revisionProperty.ToInt();
            
            // Вывести результат.
            Console.WriteLine($"Revision (as int): {revisionValue}");

            // Сохраните книгу
            workbook.Save("DocumentPropertyToIntExample.xlsx");
        }
    }
}
```

### См. также

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


