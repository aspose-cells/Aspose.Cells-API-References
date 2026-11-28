---
title: "HtmlSaveOptions.EnableCssCustomProperties"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. HTML çıktısını CSS özel özelliklerini kullanarak optimize eder. Örneğin, bir base64 görüntüsü için özel bir özellik ile birden fazla tekrar olduğunda, görüntü verisi yalnızca bir kez kaydedilir, böylece ortaya çıkan HTML'in performansı artırılabilir. Varsayılan değer false'tur."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/enablecsscustomproperties/
---
## HtmlSaveOptions.EnableCssCustomProperties property

HTML çıktısını CSS özel özellikleri kullanarak optimize eder. Örneğin, bir base64 görüntünün birden çok kez kullanıldığı senaryoda, özel özellik sayesinde görüntü verisi sadece bir kez kaydedilir ve ortaya çıkan HTML'nin performansı artırılabilir. Varsayılan değer false'tur.

```csharp
public bool EnableCssCustomProperties { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class HtmlSaveOptionsPropertyEnableCssCustomPropertiesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Biçimlendirilmiş örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A1"].GetStyle().Font.Color = System.Drawing.Color.Red;

            // Birden çok hücrede tekrarlanacak bir resim ekleyin
            int imgIndex = worksheet.Pictures.Add(1, 1, "logo.png");
            Picture pic = worksheet.Pictures[imgIndex];
            pic.Move(1, 1); // Using Move instead of LeftOffset/TopOffset
            pic.Width = 100;
            pic.Height = 100;

            // Resmi başka bir konuma kopyalayın
            worksheet.Cells["D5"].PutValue("Same image reference:");
            int imgIndex2 = worksheet.Pictures.Add(5, 3, "logo.png");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            pic2.Move(5, 3); // Using Move instead of LeftOffset/TopOffset
            pic2.Width = 100;
            pic2.Height = 100;

            // HtmlSaveOptions örneği oluştur
            HtmlSaveOptions htmlOptions = new HtmlSaveOptions();

            // Mevcut değeri gösterin
            Console.WriteLine("Current EnableCssCustomProperties value: " + htmlOptions.EnableCssCustomProperties);

            // CSS çıktısını optimize etmek için true olarak ayarlayın
            htmlOptions.EnableCssCustomProperties = true;

            // CSS optimizasyonu ile kaydedin
            workbook.Save("HtmlWithCssCustomProperties.html", htmlOptions);

            // Karşılaştırma için false olarak ayarlayın
            htmlOptions.EnableCssCustomProperties = false;
            workbook.Save("HtmlWithoutCssCustomProperties.html", htmlOptions);

            Console.WriteLine("Files saved with and without CSS custom properties optimization.");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


