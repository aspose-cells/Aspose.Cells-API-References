---
title: "Sınıf WebExtensionReference"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.WebExtensions.WebExtensionReference sınıfı. Uzantının sağlayıcı konumunu ve sürümünü tanımlar."
type: docs
url: /tr/net/aspose.cells.webextensions/webextensionreference/
---
## WebExtensionReference class

Uzantının sağlayıcı konumunu ve sürümünü tanımlamayı temsil eder.

```csharp
public class WebExtensionReference
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Id](../../aspose.cells.webextensions/webextensionreference/id/) { get; set; } | Bir katalog sağlayıcısı içinde Office Eklentisi ile ilişkili tanımlayıcıyı alır ve ayarlar. Tanımlayıcı, bir katalog sağlayıcısı içinde benzersiz OLMALIdır. |
| [StoreName](../../aspose.cells.webextensions/webextensionreference/storename/) { get; set; } | Office Eklentisinin depolandığı pazar yerinin örneğini alır ve ayarlar. |
| [StoreType](../../aspose.cells.webextensions/webextensionreference/storetype/) { get; set; } | Depolama özniteliğinin tanımladığı pazar yeri türünü alır ve ayarlar. |
| [Version](../../aspose.cells.webextensions/webextensionreference/version/) { get; set; } | Sürümü alır ve ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionReferenceDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Önce bir WebExtension oluşturun
                WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
                int extensionIndex = webExtensions.Add();
                WebExtension webExt = webExtensions[extensionIndex];

                // WebExtension'dan WebExtensionReference'ı alın
                WebExtensionReference webExtensionRef = webExt.Reference;

                // WebExtensionReference'ın özelliklerini ayarlayın
                webExtensionRef.Id = "my-addin-123";
                webExtensionRef.Version = "1.0.0";
                webExtensionRef.StoreName = "MyAddinStore";
                webExtensionRef.StoreType = WebExtensionStoreType.OMEX;

                // Referans özelliklerini görüntüleyin
                Console.WriteLine($"WebExtension Reference created:");
                Console.WriteLine($"ID: {webExtensionRef.Id}");
                Console.WriteLine($"Version: {webExtensionRef.Version}");
                Console.WriteLine($"Store Name: {webExtensionRef.StoreName}");
                Console.WriteLine($"Store Type: {webExtensionRef.StoreType}");

                // Çalışma kitabını kaydedin
                workbook.Save("WebExtensionReferenceDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with WebExtension reference.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebExtensionReference: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


