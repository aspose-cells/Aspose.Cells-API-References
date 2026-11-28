---
title: "WriteProtection.Password"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WriteProtection özelliği. Dosyayı değiştirmek için koruma parolasını ayarlar"
type: docs
url: /tr/net/aspose.cells/writeprotection/password/
---
## WriteProtection.Password property

Dosyayı değiştirmek için koruma şifresini ayarlar.

```csharp
public string Password { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyPasswordDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Yazma koruma parolasını ayarlayın
            workbook.Settings.WriteProtection.Password = "owner";
            
            // Çalışma kitabını kaydedin
            workbook.Save("WriteProtectedWorkbook.xlsx");
            
            Console.WriteLine("Workbook write-protected with password successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


