---
title: "Protection.GetPasswordHash"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Protection yöntemi. Mevcut parolanın hash'ini alır"
type: docs
url: /tr/net/aspose.cells/protection/getpasswordhash/
---
## Protection.GetPasswordHash method

Mevcut şifrenin hash değerini alır.

```csharp
public int GetPasswordHash()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionMethodGetPasswordHashDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Parola ile koruma ayarlarını ayarla
            Protection protection = worksheet.Protection;
            protection.Password = "password123";
            protection.AllowDeletingColumn = true;
            protection.AllowFormattingCell = true;
            
            // Çalışma sayfasını koru
            worksheet.Protect(ProtectionType.All);

            try
            {
                // Parola hash'ini al
                int passwordHash = protection.GetPasswordHash();
                
                // Sonucu göster
                Console.WriteLine($"Password hash: {passwordHash}");
                Console.WriteLine($"Is protected with password: {protection.IsProtectedWithPassword}");

                // Parolayı doğrula (ilgili işlevselliği göstererek)
                bool isVerified = protection.VerifyPassword("password123");
                Console.WriteLine($"Password verification result: {isVerified}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetPasswordHash method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("ProtectionMethodGetPasswordHashDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


