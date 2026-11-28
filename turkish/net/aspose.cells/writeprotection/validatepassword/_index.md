---
title: "WriteProtection.ValidatePassword"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WriteProtection yöntemi. Belirtilen parola, dosyanın yazma koruması için kullanılan parolaya aynıysa true döndürür"
type: docs
url: /tr/net/aspose.cells/writeprotection/validatepassword/
---
## WriteProtection.ValidatePassword method

Belirtilen şifrenin, dosyanın koruma şifresiyle aynı olup olmadığını true döndürür.

```csharp
public bool ValidatePassword(string password)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| parola | String | Belirtilen parola. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionMethodValidatePasswordWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Yazma koruma parolasını ayarlayın
            workbook.Settings.WriteProtection.Password = "1234";
            
            // Parolayı doğrula
            Console.WriteLine("Password '1234' is valid: " + 
                workbook.Settings.WriteProtection.ValidatePassword("1234"));
            Console.WriteLine("Password 'wrong' is valid: " + 
                workbook.Settings.WriteProtection.ValidatePassword("wrong"));
        }
    }
}
```

### Ayrıca Bakınız

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


