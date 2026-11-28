---
title: "Sınıf WriteProtection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.WriteProtection sınıfı. Bir çalışma kitabı için yazma koruma ayarlarını belirtir"
type: docs
url: /tr/net/aspose.cells/writeprotection/
---
## WriteProtection class

Bir çalışma kitabı için yazma koruma ayarlarını belirtir.

```csharp
public class WriteProtection
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Author](../../aspose.cells/writeprotection/author/) { get; set; } | Yazarı alır ve ayarlar. |
| [IsWriteProtected](../../aspose.cells/writeprotection/iswriteprotected/) { get; } | Bu çalışma kitabının yazma korumalı olup olmadığını gösterir. |
| [Password](../../aspose.cells/writeprotection/password/) { get; set; } | Dosyayı değiştirmek için koruma şifresini ayarlar. |
| [RecommendReadOnly](../../aspose.cells/writeprotection/recommendreadonly/) { get; set; } | Okunabilirlik önerilen seçeneğinin seçili olup olmadığını gösterir. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [ValidatePassword](../../aspose.cells/writeprotection/validatepassword/)(string) | Belirtilen şifrenin, dosyanın koruma şifresiyle aynı olup olmadığını true döndürür. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WriteProtectionDemo
    {
        public static void WriteProtectionExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabının ayarlarına eriş
            WorkbookSettings settings = workbook.Settings;

            // Yazma koruma ayarlarına eriş
            WriteProtection writeProtection = settings.WriteProtection;

            // Yazma korumasının yazarını ayarla
            writeProtection.Author = "John Doe";

            // Yazma koruması için şifreyi ayarla
            writeProtection.Password = "password123";

            // Önerilen yalnızca okuma seçeneğini ayarla
            writeProtection.RecommendReadOnly = true;

            // Çalışma kitabının yazma korumalı olup olmadığını kontrol et
            bool isWriteProtected = writeProtection.IsWriteProtected;
            Console.WriteLine("Is Write Protected: " + isWriteProtected);

            // Şifreyi doğrula
            bool isValidPassword = writeProtection.ValidatePassword("password123");
            Console.WriteLine("Is Valid Password: " + isValidPassword);

            // Çalışma kitabını kaydedin
            workbook.Save("WriteProtectionExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


