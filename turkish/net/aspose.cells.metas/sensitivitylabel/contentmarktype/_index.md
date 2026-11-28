---
title: "SensitivityLabel.ContentMarkType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SensitivityLabel özelliği. Bir dosyaya uygulanması gereken içerik işaretleme türlerini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.metas/sensitivitylabel/contentmarktype/
---
## SensitivityLabel.ContentMarkType property

Bir dosyaya uygulanması gereken içerik işaretleme türlerini alır ve ayarlar.

```csharp
public SensitivityLabelMarkType ContentMarkType { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyContentMarkTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // Bir duyarlılık etiketi örneği oluşturun
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // Temel özellikleri ayarlayın
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;
                
                // ContentMarkType özelliğini gösterin (okuma-yazma)
                Console.WriteLine("Initial ContentMarkType: " + label.ContentMarkType);
                
                // Farklı içerik işaretleme türlerini ayarlayın
                label.ContentMarkType = SensitivityLabelMarkType.Header;
                Console.WriteLine("After setting Header: " + label.ContentMarkType);
                
                label.ContentMarkType = SensitivityLabelMarkType.Watermark;
                Console.WriteLine("After setting Watermark: " + label.ContentMarkType);
                
                // Birleştirilmiş bayrak kullanımını gösterin
                label.ContentMarkType = SensitivityLabelMarkType.Header | SensitivityLabelMarkType.Footer;
                Console.WriteLine("Combined Header+Footer: " + label.ContentMarkType);
                
                // Çalışma kitabını kaydedin
                workbook.Save("ContentMarkTypeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [SensitivityLabelMarkType](../../sensitivitylabelmarktype/)
* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


