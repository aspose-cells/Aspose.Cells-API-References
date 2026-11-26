---
title: "Workbook.AcceptAllRevisions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Принимает все отслеживаемые изменения в рабочей книге"
type: docs
url: /ru/net/aspose.cells/workbook/acceptallrevisions/
---
## Workbook.AcceptAllRevisions method

Принимает все отслеживаемые изменения в рабочей книге.

```csharp
public void AcceptAllRevisions()
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodAcceptAllRevisionsDemo
    {
        public static void Run()
        {
            // Создать рабочую книгу с изменениями
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить несколько изменений (отслеживание изменений должно быть включено в Excel сначала)
            worksheet.Cells["A1"].PutValue("Original Value");
            
            // Сохранить с изменениями
            string sourcePath = "source_with_revisions.xlsx";
            workbook.Save(sourcePath, SaveFormat.Xlsx);
            
            // Повторно открыть рабочую книгу
            workbook = new Workbook(sourcePath);
            
            // Проверить наличие изменений и принять их
            if (workbook.HasRevisions)
            {
                Console.WriteLine("Workbook has revisions. Accepting all...");
                workbook.AcceptAllRevisions();
                
                // Сохранить без изменений
                string destPath = "output_no_revisions.xlsx";
                workbook.Save(destPath, SaveFormat.Xlsx);
                Console.WriteLine("Revisions accepted and saved to: " + destPath);
            }
            else
            {
                Console.WriteLine("Workbook has no revisions.");
            }
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


