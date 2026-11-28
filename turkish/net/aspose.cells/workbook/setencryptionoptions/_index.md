---
title: "Workbook.SetEncryptionOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Şifreleme Seçeneklerini Ayarla"
type: docs
url: /tr/net/aspose.cells/workbook/setencryptionoptions/
---
## Workbook.SetEncryptionOptions method

Şifreleme Seçeneklerini Ayarla.

```csharp
public void SetEncryptionOptions(EncryptionType encryptionType, int keyLength)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| encryptionType | EncryptionType | Şifreleme türü. |
| keyLength | Int32 | Anahtar uzunluğu. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSetEncryptionOptionsWithEncryptionTypeInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma sayfasına bazı veriler ekle
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Encryption");
            
            // Parola ve şifreleme seçeneklerini ayarlayın
            workbook.Settings.Password = "1234";
            workbook.SetEncryptionOptions(EncryptionType.StrongCryptographicProvider, 128);
            
            // Şifrelenmiş çalışma kitabını kaydedin
            workbook.Save("EncryptedWorkbook.xls", SaveFormat.Excel97To2003);
            
            // Şifrelenmiş çalışma kitabını yükleyerek doğrulayın
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.Password = "1234";
            Workbook encryptedWorkbook = new Workbook("EncryptedWorkbook.xls", loadOptions);
            
            Console.WriteLine("Workbook encrypted and loaded successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* enum [EncryptionType](../../encryptiontype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


