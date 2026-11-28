---
title: "Worksheet.Unprotect"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Çalışma sayfasının korumasını kaldırır."
type: docs
url: /tr/net/aspose.cells/worksheet/unprotect/
---
## Unprotect() {#unprotect}

Çalışma sayfasının korumasını kaldırır.

```csharp
public void Unprotect()
```

### Açıklamalar

Bu yöntem, şifresiz korunan çalışma sayfasının korumasını kaldırır.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodUnprotectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasını bir şifreyle koru
            worksheet.Protect(ProtectionType.All, "password123", null);
            Console.WriteLine("Worksheet is protected: " + worksheet.IsProtected);
            
            try
            {
                // Şifresiz çalışma sayfasının korumasını kaldır (başarısız olmalı)
                worksheet.Unprotect();
                Console.WriteLine("Worksheet unprotected without password: " + !worksheet.IsProtected);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error when trying to unprotect without password: " + ex.Message);
            }

            try
            {
                // Yanlış şifreyle çalışma sayfasının korumasını kaldır (başarısız olmalı)
                worksheet.Unprotect("wrongpassword");
                Console.WriteLine("Worksheet unprotected with wrong password: " + !worksheet.IsProtected);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error when trying to unprotect with wrong password: " + ex.Message);
            }

            try
            {
                // Çalışma sayfasının korumasını doğru şifreyle kaldır
                worksheet.Unprotect("password123");
                Console.WriteLine("Worksheet successfully unprotected: " + !worksheet.IsProtected);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error when trying to unprotect: " + ex.Message);
            }
            
            // Sonucu kaydet
            workbook.Save("WorksheetMethodUnprotectDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Unprotect(string) {#unprotect_1}

Çalışma sayfasının korumasını kaldırır.

```csharp
public void Unprotect(string password)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| parola | String | Şifre |

### Açıklamalar

Çalışma sayfası şifresiz korumalıysa, şifre parametresine null değer veya boş dize ayarlayabilirsiniz.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodUnprotectWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasını şifre ve varsayılan koruma türüyle koru
            worksheet.Protect(ProtectionType.All, "test", null);
            
            // Çalışma sayfasının korumasını şifreyle kaldır
            worksheet.Unprotect("test");
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


