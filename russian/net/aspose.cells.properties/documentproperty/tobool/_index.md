---
title: "DocumentProperty.ToBool"
second_title: "Справочник API Aspose.Cells для .NET"
description: "DocumentProperty method. Возвращает значение свойства как bool"
type: docs
url: /ru/net/aspose.cells.properties/documentproperty/tobool/
---
## DocumentProperty.ToBool method

Возвращает значение свойства как bool.

```csharp
public bool ToBool()
```

### Примечания

Выбрасывает исключение, если тип свойства не PropertyType.Boolean.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToBoolDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Добавьте булевое пользовательское свойство документа
            customProperties.Add("IsApproved", true);
            
            // Получите свойство и преобразуйте в bool, используя ToBool()
            DocumentProperty isApprovedProperty = customProperties["IsApproved"];
            bool isApproved = isApprovedProperty.ToBool();
            
            Console.WriteLine($"Is Approved: {isApproved}");
        }
    }
}
```

### См. также

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


