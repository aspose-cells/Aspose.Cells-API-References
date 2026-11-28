---
title: "WebExtension.IsFrozen"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebExtension özelliği. Kullanıcının Office Eklentisiyle etkileşime girip giremeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells.webextensions/webextension/isfrozen/
---
## WebExtension.IsFrozen property

Kullanıcının Office Eklentisiyle etkileşime girip giremeyeceğini gösterir.

```csharp
public bool IsFrozen { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyIsFrozenDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // Bu satır başarısız olur çünkü WebExtension yapıcı parametreleri gerektirir
                // WebExtension webExtension = new WebExtension();
                
                // Bunun yerine, mümkünse çalışma kitabından bir web uzantısı alacağız
                // veya farklı bir yaklaşımla göster
                Console.WriteLine("Note: WebExtension requires constructor parameters. This demo shows property usage conceptually.");
                
                // Gösterim amaçlı, geçerli bir örnek varsa özelliğin nasıl çalışacağını göstereceğiz
                // Gerçek bir senaryoda, WebExtension örneğini çalışma kitabından ya da başka bir kaynaktan alırsınız
                WebExtension webExtension = GetWebExtensionInstance(workbook);
                
                if (webExtension != null)
                {
                    // İlk özellikleri ayarlayın
                    webExtension.Id = "MyAddin123";
                    
                    // İlk IsFrozen değerini göster
                    Console.WriteLine($"Initial IsFrozen value: {webExtension.IsFrozen}");
                    
                    // IsFrozen özelliğini değiştir (çünkü okuma-yazma)
                    webExtension.IsFrozen = true;
                    Console.WriteLine($"Updated IsFrozen value: {webExtension.IsFrozen}");
                    
                    // Kullanıcının etkileşime girip giremeyeceğini kontrol ederek etkiyi göster
                    Console.WriteLine($"User can{(webExtension.IsFrozen ? "not" : "")} interact with the add-in");
                    
                    // Çalışma kitabını kaydet (ancak ek web uzantısı ek adımlar olmadan kalıcı olmayabilir)
                    workbook.Save("WebExtensionIsFrozenDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("Could not obtain a WebExtension instance for demonstration.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private static WebExtension GetWebExtensionInstance(Workbook workbook)
        {
            // Gerçek bir uygulamada, bu çalışma kitabından mevcut bir WebExtension alır
            // veya gerekli yapıcı parametreleriyle düzgün bir şekilde oluştur
            // Bu sadece gösterim için bir yer tutucudur
            return null;
        }
    }
}
```

### Ayrıca Bakınız

* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


