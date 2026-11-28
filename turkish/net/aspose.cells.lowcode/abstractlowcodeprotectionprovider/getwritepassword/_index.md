---
title: "AbstractLowCodeProtectionProvider.GetWritePassword"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AbstractLowCodeProtectionProvider yöntemi. Elektronik tablo dosyasını değiştirmek için parolayı alır"
type: docs
url: /tr/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getwritepassword/
---
## AbstractLowCodeProtectionProvider.GetWritePassword method

Elektronik tablo dosyasını değiştirmek için şifreyi alır.

```csharp
public virtual string GetWritePassword()
```

### Dönüş Değeri

Elektronik tablo dosyasını değiştirmek için parola. Boş, dosyanın değiştirilmesi için koruma olmadığını gösterir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWritePasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Özel koruma sağlayıcı örneği oluştur
            var protectionProvider = new CustomProtectionProvider();

            try
            {
                // GetWritePassword yöntemini açıkça çağırın ve sonucu gösterin
                string writePassword = protectionProvider.GetWritePassword();
                Console.WriteLine($"Retrieved write password: {writePassword}");

                // Çalışma kitabını kaydedin - yazma korumasını doğrudan uygulayın
                workbook.Settings.WriteProtection.Password = writePassword;
                workbook.Save("MethodGetWritePasswordDemo.xlsx");
                Console.WriteLine("Workbook saved with write protection password.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetWritePassword method: {ex.Message}");
            }
        }

    }

    // Özel koruma sağlayıcı uygulaması
    public class CustomProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public override string GetWritePassword()
        {
            return "AsposeTestPassword123!";
        }

        // Diğer gerekli yöntemleri varsayılan dönüşlerle uygulayın
        public override string GetOpenPassword() => null;
        public override string GetWorkbookPassword() => null;
        public override ProtectionType GetWorkbookProtectionType() => ProtectionType.None;
        public override string GetWorksheetPassword(string sheetName) => null;
        public override ProtectionType GetWorksheetProtectionType(string sheetName) => ProtectionType.None;
    }
}
```

### Ayrıca Bakınız

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


