---
title: "Worksheet.IsProtected"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Çalışma sayfasının korumalı olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/worksheet/isprotected/
---
## Worksheet.IsProtected property

Çalışma sayfasının korumalı olup olmadığını gösterir.

```csharp
public bool IsProtected { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsProtectedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma kitabını ve ilk çalışma sayfasını koru
            workbook.Protect(ProtectionType.All, "password");
            workbook.Worksheets[0].Protect(ProtectionType.All, "password", null);

            // Çalışma sayfasının korumalı olup olmadığını kontrol edin
            bool isProtected = workbook.Worksheets[0].IsProtected;
            Console.WriteLine($"Worksheet is protected: {isProtected}");

            // Çalışma kitabını kaydedin
            workbook.Save("protected_worksheet.xlsx");

            // Kaydedilmiş çalışma kitabını yükleyin ve korumayı doğrulayın
            Workbook loadedWorkbook = new Workbook("protected_worksheet.xlsx");
            Console.WriteLine($"Loaded worksheet is protected: {loadedWorkbook.Worksheets[0].IsProtected}");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


