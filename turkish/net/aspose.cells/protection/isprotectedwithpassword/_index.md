---
title: "Protection.IsProtectedWithPassword"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Protection özelliği. Çalışma sayfasının şifreyle korunup korunmadığını gösterir."
type: docs
url: /tr/net/aspose.cells/protection/isprotectedwithpassword/
---
## Protection.IsProtectedWithPassword property

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
    public class ProtectionPropertyIsProtectedWithPasswordDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfası koruma ayarlarına erişin.
            Protection protection = worksheet.Protection;

            // Koruma şifresini ayarlayın
            protection.Password = "test123";

            // Çalışma sayfasının şifreyle korunup korunmadığını kontrol edin
            bool isProtectedWithPassword = protection.IsProtectedWithPassword;
            Console.WriteLine("Is worksheet protected with password: " + isProtectedWithPassword);

            // Çalışma kitabını kaydedin
            workbook.Save("PasswordProtectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


