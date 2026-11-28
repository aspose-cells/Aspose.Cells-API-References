---
title: "Workbook.AcceptAllRevisions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Çalışma kitabındaki tüm izlenen değişiklikleri kabul eder"
type: docs
url: /tr/net/aspose.cells/workbook/acceptallrevisions/
---
## Workbook.AcceptAllRevisions method

Çalışma kitabındaki tüm izlenen değişiklikleri kabul eder.

```csharp
public void AcceptAllRevisions()
```

### Örnekler

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
            // Değişiklikli bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bazı değişiklikler ekle (izleme değişiklikleri önce Excel'de etkinleştirilmelidir)
            worksheet.Cells["A1"].PutValue("Original Value");
            
            // Değişikliklerle kaydet
            string sourcePath = "source_with_revisions.xlsx";
            workbook.Save(sourcePath, SaveFormat.Xlsx);
            
            // Çalışma kitabını yeniden aç
            workbook = new Workbook(sourcePath);
            
            // Değişikliklerin olup olmadığını kontrol et ve kabul et
            if (workbook.HasRevisions)
            {
                Console.WriteLine("Workbook has revisions. Accepting all...");
                workbook.AcceptAllRevisions();
                
                // Değişiklik olmadan kaydet
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

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


