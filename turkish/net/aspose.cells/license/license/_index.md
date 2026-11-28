---
title: "License.License"
second_title: "Aspose.Cells için .NET API Referansı"
description: "License yapıcı. Bu sınıfın yeni bir örneğini başlatır"
type: docs
url: /tr/net/aspose.cells/license/license/
---
## License constructor

Bu sınıfın yeni bir örneğini başlatır.

```csharp
public License()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LicenseMethodCtorDemo
    {
        public static void Run()
        {
            // Yapıcıyı (#ctor) kullanarak License'ın yeni bir örneğini oluştur
            License license = new License();
            
            // Lisans dosyasını ayarla
            license.SetLicense("MyLicense.lic");
            
            Console.WriteLine("License set successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [License](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


