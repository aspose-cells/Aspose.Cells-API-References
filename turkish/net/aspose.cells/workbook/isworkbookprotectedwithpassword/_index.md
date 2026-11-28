---
title: "Workbook.IsWorkbookProtectedWithPassword"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook özelliği. Yapının ya da pencerenin şifreyle korunup korunmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/workbook/isworkbookprotectedwithpassword/
---
## Workbook.IsWorkbookProtectedWithPassword property

Yapının veya pencerenin parola ile korunup korunmadığını gösterir.

```csharp
public bool IsWorkbookProtectedWithPassword { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyIsWorkbookProtectedWithPasswordDemo
    {
        public static void Run()
        {
            // Yeni bir Workbook örneği oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabının şifreyle korunup korunmadığını kontrol et (yeni çalışma kitabı için false olmalı)
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Çalışma kitabını bir şifreyle koru
            workbook.Protect(ProtectionType.All, "password123");

            // Şimdi tekrar kontrol et (true olmalı)
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Çalışma kitabının korumasını kaldır
            workbook.Unprotect("password123");

            // Son kontrol (tekrar false olmalı)
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Çalışma kitabını serbest bırak
            workbook.Dispose();
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


