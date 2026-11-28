---
title: "AbstractLowCodeProtectionProvider.GetOpenPassword"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AbstractLowCodeProtectionProvider yöntemi. Elektronik tablo dosyasını açmak için şifreyi alır"
type: docs
url: /tr/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getopenpassword/
---
## AbstractLowCodeProtectionProvider.GetOpenPassword method

Elektronik tablo dosyasını açmak için şifreyi alır.

```csharp
public virtual string GetOpenPassword()
```

### Dönüş Değeri

Elektronik tablo dosyasını açmak için şifre. Boş olması, dosyayı açmak için koruma olmadığını gösterir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetOpenPasswordDemo
    {
        public static void Run()
        {
            try
            {
                // Bir koruma sağlayıcı örneği oluştur
                var protectionProvider = new DemoProtectionProvider();

                // Parolayı almak için GetOpenPassword yöntemini çağırın
                string password = protectionProvider.GetOpenPassword();

                // Yeni bir çalışma kitabı oluşturun ve parolayı uygulayın
                Workbook workbook = new Workbook("sample.xlsx");
                workbook.Settings.Password = password;

                // Parola korumalı çalışma kitabını kaydedin
                workbook.Save("MethodGetOpenPasswordDemo.xlsx");

                Console.WriteLine($"Workbook protected with open password: {password}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing demo: {ex.Message}");
            }
        }
    }

    public class DemoProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public override string GetOpenPassword()
        {
            return "AsposeDemo123!";
        }
    }
}
```

### Ayrıca Bakınız

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


