---
title: "ImageOrPrintOptions.IsCellAutoFit"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageOrPrintOptions özelliği. Hücrelerin genişlik ve yüksekliğinin hücre değeriyle otomatik olarak ayarlanıp ayarlanmadığını gösterir. Varsayılan değer false"
type: docs
url: /tr/net/aspose.cells.rendering/imageorprintoptions/iscellautofit/
---
## ImageOrPrintOptions.IsCellAutoFit property

Hücrelerin genişlik ve yüksekliğinin hücre değeriyle otomatik olarak ayarlanıp ayarlanmadığını gösterir. Varsayılan değer false.

```csharp
[Obsolete("This property is not used, please remove this property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsCellAutoFit { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine, bu özellik kullanılmaz, lütfen bu özelliği kaldırın. Bu özellik Ağustos 2022'den itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyIsCellAutoFitDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasına erişin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Varsayılan sütun genişliğini aşan örnek metni ayarlayın
            worksheet.Cells["B4"].Value = "This is a long text that demonstrates cell autofit behavior when converting to image.";
            
            // Görüntü renderleme seçeneklerini oluştur
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // IsCellAutoFit false (varsayılan) gösterin
            Console.WriteLine("Default IsCellAutoFit value: " + options.IsCellAutoFit);
            SaveAsImage(worksheet, options, "WithoutAutoFit.png");

            // IsCellAutoFit'i true olarak değiştirin
            options.IsCellAutoFit = true;
            Console.WriteLine("Modified IsCellAutoFit value: " + options.IsCellAutoFit);
            SaveAsImage(worksheet, options, "WithAutoFit.png");

            Console.WriteLine("Images created successfully. Compare column widths in output files.");
        }

        private static void SaveAsImage(Worksheet worksheet, ImageOrPrintOptions options, string fileName)
        {
            // Görüntü biçimini yapılandırın
            options.ImageType = ImageType.Png;

            // Çalışma sayfasını belirtilen seçeneklerle görüntüye renderlayın
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, fileName);
        }
    }
}
```

### Ayrıca Bakınız

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


