---
title: "AbstractLowCodeProtectionProvider.GetWorksheetPassword"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AbstractLowCodeProtectionProvider yöntemi. Belirtilen çalışma sayfasını korumak için parolayı alır"
type: docs
url: /tr/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetpassword/
---
## AbstractLowCodeProtectionProvider.GetWorksheetPassword method

Belirtilen çalışma sayfasını korumak için şifreyi alır.

```csharp
public virtual string GetWorksheetPassword(string sheetName)
```

### Dönüş Değeri

Belirtilen çalışma sayfasını korumak için parola.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWorksheetPasswordWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasına erişin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            string sheetName = worksheet.Name;

            // Özel koruma sağlayıcı örneği oluştur
            var provider = new CustomProtectionProvider();

            try
            {
                // Çalışma sayfası adıyla GetWorksheetPassword yöntemini çağırın
                string password = provider.GetWorksheetPassword(sheetName);

                // Alınan parolayı kullanarak çalışma sayfasına koruma uygulayın
                worksheet.Protect(ProtectionType.All, password, null);

                Console.WriteLine($"Protected worksheet '{sheetName}' with password: {password}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetWorksheetPassword: {ex.Message}");
            }

            // Korunan çalışma kitabını kaydet
            workbook.Save("WorksheetPasswordDemo.xlsx");

        }
    }

    // Sayfa adına göre parola döndüren özel uygulama
    public class CustomProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public new string GetWorksheetPassword(string sheetName)
        {
            // Gösterim için basit parola oluşturma mantığı
            return $"pw_{sheetName}";
        }
    }
}
```

### Ayrıca Bakınız

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


