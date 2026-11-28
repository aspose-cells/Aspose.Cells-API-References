---
title: "LoadOptions.Password"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadOptions özelliği. Çalışma kitabının şifresini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/loadoptions/password/
---
## LoadOptions.Password property

Çalışma kitabının şifresini alır ve ayarlar.

```csharp
public string Password { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyPasswordDemo
    {
        public static void Run()
        {
            // Yükleme seçeneklerini oluştur ve şifreyi ayarla
            LoadOptions options = new LoadOptions();
            options.Password = "test";

            // Şifre korumalı çalışma kitabını yükle
            Workbook workbook = new Workbook("protected.xlsx", options);

            // Yükledikten sonra şifre korumasını kaldır
            workbook.Settings.Password = null;

            // Korumasız çalışma kitabını kaydedin
            workbook.Save("unprotected.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


