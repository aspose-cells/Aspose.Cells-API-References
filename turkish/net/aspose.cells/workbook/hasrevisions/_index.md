---
title: "Workbook.HasRevisions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook özelliği. Çalışma kitabının izlenen değişiklikleri olup olmadığını alır"
type: docs
url: /tr/net/aspose.cells/workbook/hasrevisions/
---
## Workbook.HasRevisions property

Çalışma kitabının izlenen değişiklikleri olup olmadığını alır.

```csharp
public bool HasRevisions { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyHasRevisionsDemo
    {
        public static void Run()
        {
            // Değişiklikli bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir revizyon oluşturacak bir değişiklik yap
            worksheet.Cells["A1"].PutValue("Original Value");
            
            // Çalışma kitabının revizyonları olup olmadığını kontrol et
            Console.WriteLine("Workbook has revisions: " + workbook.HasRevisions);
            
            // Tüm revizyonları kabul et (varsa)
            if (workbook.HasRevisions)
            {
                workbook.AcceptAllRevisions();
            }
            
            // Revizyonları kabul ettikten sonra tekrar kontrol et
            Console.WriteLine("Workbook has revisions after accepting: " + workbook.HasRevisions);
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


