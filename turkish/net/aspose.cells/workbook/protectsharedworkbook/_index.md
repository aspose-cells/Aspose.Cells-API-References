---
title: "Workbook.ProtectSharedWorkbook"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Paylaşılan bir çalışma kitabını korur"
type: docs
url: /tr/net/aspose.cells/workbook/protectsharedworkbook/
---
## Workbook.ProtectSharedWorkbook method

Paylaşılan bir çalışma kitabını korur.

```csharp
public void ProtectSharedWorkbook(string password)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| parola | String | Çalışma kitabını korumak için şifre. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodProtectSharedWorkbookWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // Paylaşılan çalışma kitabını şifreyle koru
            wb.ProtectSharedWorkbook("abcd");
            
            // Korunan çalışma kitabını kaydet
            wb.Save("ProtectedSharedWorkbook.xlsx");
            
            // Korunan çalışma kitabını yükle
            Workbook wbProtected = new Workbook("ProtectedSharedWorkbook.xlsx");
            
            // Koruma durumunu doğrula
            Console.WriteLine("Workbook is protected: " + wbProtected.Settings.IsProtected);
            
            // Çalışma kitabının korumasını kaldır
            wbProtected.UnprotectSharedWorkbook("abcd");
            
            // Korumasız çalışma kitabını kaydedin
            wbProtected.Save("UnprotectedSharedWorkbook.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


