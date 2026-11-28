---
title: "EncryptionType enum"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.EncryptionType enum. Şifreleme Türü. Yalnızca excel2003 tarafından kullanılır. 2007/2010 çalışma kitabını Excel'in yaptığı gibi SHA AES kullanarak şifreleyeceğiz ve bu EncryptionType yok sayılacak."
type: docs
url: /tr/net/aspose.cells/encryptiontype/
---
## EncryptionType enumeration

Şifreleme Türü. Yalnızca excel2003 tarafından kullanılır. Excel'in yaptığı gibi SHA AES kullanarak 2007/2010 çalışma kitabını şifreleyeceğiz ve bu EncryptionType yok sayılacaktır.

```csharp
public enum EncryptionType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| XOR | `0` | XOR şifreleme algoritması. |
| Compatible | `1` | Office 97/2000 uyumlu. |
| EnhancedCryptographicProviderV1 | `2` | Gelişmiş şifreleme. |
| StrongCryptographicProvider | `3` | Güçlü şifreleme algoritması. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class EncryptionTypeDemo
    {
        public static void EncryptionTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabı için şifreleme seçeneklerini ayarla
            EncryptionType encryptionType = EncryptionType.EnhancedCryptographicProviderV1;
            int keyLength = 128; // Key length can be 40, 128, or 256 bits

            // Şifreleme ayarlarını uygula
            workbook.SetEncryptionOptions(encryptionType, keyLength);

            // Çalışma kitabını bir şifreyle koru
            string password = "securePassword";
            workbook.Protect(ProtectionType.All, password);

            // Çalışma kitabını kaydedin
            workbook.Save("EncryptedWorkbook.xlsx");
            workbook.Save("EncryptedWorkbook.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


