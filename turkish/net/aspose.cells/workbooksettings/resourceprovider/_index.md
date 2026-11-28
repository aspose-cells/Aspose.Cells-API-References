---
title: "WorkbookSettings.ResourceProvider"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. LinkToFile türündeki resim verilerini yükleme gibi harici kaynaklar için akış sağlayıcısını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/workbooksettings/resourceprovider/
---
## WorkbookSettings.ResourceProvider property

Harici kaynak için akış sağlayıcısını alır ve ayarlar, örneğin "LinkToFile" türündeki resim verisini yüklemek gibi.

```csharp
public IStreamProvider ResourceProvider { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyResourceProviderDemo
    {
        public static void Run()
        {
            // Örnek bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Kaynak sağlayıcıyı göstermek için bir örnek şekil ekleyin
            worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 200);
            
            // Kaynak sağlayıcıyı ayarlayın
            workbook.Settings.ResourceProvider = new MemoryStreamProvider();
            
            // Şekli, kaynak sağlayıcıyı kullanarak resim olarak kaydedin
            string outputPath = "output_shape.png";
            worksheet.Shapes[0].ToImage(outputPath, new ImageOrPrintOptions());
            
            Console.WriteLine("Shape saved as image using ResourceProvider.");
        }
    }

    public class MemoryStreamProvider : IStreamProvider
    {
        public void CloseStream(StreamProviderOptions options)
        {
            options.Stream.Close();
        }

        public void InitStream(StreamProviderOptions options)
        {
            options.Stream = new FileStream(options.DefaultPath, FileMode.Create);
        }
    }
}
```

### Ayrıca Bakınız

* interface [IStreamProvider](../../istreamprovider/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


