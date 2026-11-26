---
title: "Workbook.HasRevisions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Workbook. Возвращает, есть ли в книге отслеживаемые изменения"
type: docs
url: /ru/net/aspose.cells/workbook/hasrevisions/
---
## Workbook.HasRevisions property

Получает, есть ли в рабочей книге отслеживаемые изменения

```csharp
public bool HasRevisions { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyHasRevisionsDemo
    {
        public static void Run()
        {
            // Создать рабочую книгу с изменениями
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Сделайте изменение, которое создаст ревизию
            worksheet.Cells["A1"].PutValue("Original Value");
            
            // Проверить, есть ли в книге ревизии
            Console.WriteLine("Workbook has revisions: " + workbook.HasRevisions);
            
            // Принять все ревизии (если есть)
            if (workbook.HasRevisions)
            {
                workbook.AcceptAllRevisions();
            }
            
            // Проверьте снова после принятия ревизий
            Console.WriteLine("Workbook has revisions after accepting: " + workbook.HasRevisions);
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


