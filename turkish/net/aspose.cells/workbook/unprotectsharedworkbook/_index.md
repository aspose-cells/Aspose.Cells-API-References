---
title: "Workbook.UnprotectSharedWorkbook"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Paylaşılan bir çalışma kitabının korumasını kaldırır"
type: docs
url: /tr/net/aspose.cells/workbook/unprotectsharedworkbook/
---
## Workbook.UnprotectSharedWorkbook method

Paylaşılan bir çalışma kitabının korumasını kaldırır.

```csharp
public void UnprotectSharedWorkbook(string password)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| parola | String | Çalışma kitabının korumasını kaldırmak için parola. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodUnprotectSharedWorkbookWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // Paylaşılan çalışma kitabını şifreyle koru
            wb.ProtectSharedWorkbook("abcd");
            
            // Korunan çalışma kitabını kaydet
            wb.Save("ProtectedSharedWorkbook.xlsx");
            
            // Çalışma kitabını yeniden aç
            wb = new Workbook("ProtectedSharedWorkbook.xlsx");
            
            // Şifreyle paylaşılan çalışma kitabının korumasını kaldır
            wb.UnprotectSharedWorkbook("abcd");
            
            // Korumasız çalışma kitabını kaydedin
            wb.Save("UnprotectedSharedWorkbook.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


