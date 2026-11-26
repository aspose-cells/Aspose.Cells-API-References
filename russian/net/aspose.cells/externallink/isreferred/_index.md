---
title: "ExternalLink.IsReferred"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalLink. Указывает, ссылаются ли другие объекты на эту внешнюю ссылку"
type: docs
url: /ru/net/aspose.cells/externallink/isreferred/
---
## ExternalLink.IsReferred property

Указывает, ссылаются ли другие элементы на эту внешнюю ссылку.

```csharp
public bool IsReferred { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyIsReferredDemo
    {
        public static void Run()
        {
            // Создайте рабочую книгу с внешней ссылкой
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте ссылку на внешнюю ссылку
            worksheet.Cells["A1"].Formula = "='[external.xlsx]Sheet1'!A1";
            
            // Проверьте, упомянута ли внешняя ссылка
            if (workbook.Worksheets.ExternalLinks.Count > 0)
            {
                bool isReferred = workbook.Worksheets.ExternalLinks[0].IsReferred;
                Console.WriteLine("Is external link referred: " + isReferred);
            }
        }
    }
}
```

### См. также

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


