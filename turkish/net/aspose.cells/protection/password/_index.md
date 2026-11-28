---
title: "Protection.Password"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Protection özelliği. Çalışma sayfasını korumak için kullanılan şifreyi temsil eder."
type: docs
url: /tr/net/aspose.cells/protection/password/
---
## Protection.Password property

Çalışma sayfasını korumak için kullanılan şifreyi temsil eder.

```csharp
public string Password { get; set; }
```

### Açıklamalar

Şifre null veya boş bir dize olarak ayarlanmışsa, çalışma sayfasının veya çalışma kitabının şifresini kullanmadan korumasını kaldırabilirsiniz. Aksi takdirde, çalışma sayfasının veya çalışma kitabının korumasını kaldırmak için şifreyi belirtmeniz gerekir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyPasswordDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Parola ile koruma ayarlarını ayarla
            Protection protection = worksheet.Protection;
            protection.AllowEditingContent = false;
            protection.AllowDeletingColumn = false;
            protection.Password = "test123";

            // Şifre korumasını doğrulayın
            Console.WriteLine("Worksheet is protected: " + (protection.Password != null));
            Console.WriteLine("Protection password: " + protection.Password);

            // Karşılaştırma için başka bir koruma nesnesi oluşturun
            Protection protection2 = worksheet.Protection;
            protection2.Password = "test123";

            // Şifre korumasını karşılaştırın
            Console.WriteLine("Passwords match: " + (protection.Password == protection2.Password));
        }
    }
}
```

### Ayrıca Bakınız

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


