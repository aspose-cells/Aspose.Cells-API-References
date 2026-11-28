---
title: "VbaProject.ValidatePassword"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaProject yöntemi. Koruma şifresini doğrular"
type: docs
url: /tr/net/aspose.cells.vba/vbaproject/validatepassword/
---
## VbaProject.ValidatePassword method

Koruma şifresini doğrular.

```csharp
public bool ValidatePassword(string password)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| parola | String | şifre |

### Dönüş Değeri

Şifrenin bu VBA projesinin koruma şifresi olup olmadığı

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectMethodValidatePasswordWithStringDemo
    {
        public static void Run()
        {
            // VBA projesi içeren örnek Excel dosyasından çalışma kitabı nesnesi oluşturun
            Workbook workbook = new Workbook("example.xlsm");
            
            // VBA proje şifresini doğrulayın
            bool isValid = workbook.VbaProject.ValidatePassword("test");
            
            // Doğrulama sonucunu çıktı olarak verin
            Console.WriteLine("Password validation result: " + isValid);
        }
    }
}
```

### Ayrıca Bakınız

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


