---
title: "ProtectedRange.IsProtectedWithPassword"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ProtectedRange özelliği. Çalışma sayfasının şifreyle korunup korunmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/protectedrange/isprotectedwithpassword/
---
## ProtectedRange.IsProtectedWithPassword property

Çalışma sayfasının şifre ile korunup korunmadığını gösterir.

```csharp
public bool IsProtectedWithPassword { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyIsProtectedWithPasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Korunan aralıkları oluştur ve indekslerini al
            int protectedIndex = worksheet.AllowEditRanges.Add("PasswordProtected", 0, 0, 5, 5);
            ProtectedRange protectedWithPassword = worksheet.AllowEditRanges[protectedIndex];
            protectedWithPassword.Password = "test123";
            
            int unprotectedIndex = worksheet.AllowEditRanges.Add("Unprotected", 6, 0, 11, 5);
            ProtectedRange unprotected = worksheet.AllowEditRanges[unprotectedIndex];
            
            // Çalışma sayfasını koruyarak kısıtlamaları uygula
            worksheet.Protect(ProtectionType.All);
            
            // Şifre koruma durumunu doğrula
            Console.WriteLine($"Range '{protectedWithPassword.Name}' password protected: {protectedWithPassword.IsProtectedWithPassword}");
            Console.WriteLine($"Range '{unprotected.Name}' password protected: {unprotected.IsProtectedWithPassword}");
        }
    }
}
```

### Ayrıca Bakınız

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


