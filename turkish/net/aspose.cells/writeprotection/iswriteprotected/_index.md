---
title: "WriteProtection.IsWriteProtected"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WriteProtection özelliği. Bu çalışma kitabının yazma korumalı olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/writeprotection/iswriteprotected/
---
## WriteProtection.IsWriteProtected property

Bu çalışma kitabının yazma korumalı olup olmadığını gösterir.

```csharp
public bool IsWriteProtected { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyIsWriteProtectedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Parola ile yazma korumasını etkinleştirin
            workbook.Settings.WriteProtection.Password = "1234";
            
            // Çalışma kitabının yazma korumalı olup olmadığını kontrol edin
            Console.WriteLine("Is workbook write protected? " + 
                workbook.Settings.WriteProtection.IsWriteProtected);
            
            // Şifreyi doğrula
            Console.WriteLine("Is password valid? " + 
                workbook.Settings.WriteProtection.ValidatePassword("1234"));
            
            // Çalışma kitabını kaydedin
            workbook.Save("WriteProtectedWorkbook.xlsx");
            
            // Korumanın doğrulanması için kaydedilmiş çalışma kitabını yükleyin
            Workbook loadedWorkbook = new Workbook("WriteProtectedWorkbook.xlsx");
            
            // Koruma durumunu tekrar kontrol edin
            Console.WriteLine("Is loaded workbook write protected? " + 
                loadedWorkbook.Settings.WriteProtection.IsWriteProtected);
        }
    }
}
```

### Ayrıca Bakınız

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


