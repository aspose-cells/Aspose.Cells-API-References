---
title: "SensitivityLabel.SiteId"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SensitivityLabel özelliği. Hassasiyet etiketini tanımlayan hassasiyet etiketi politikasına karşılık gelen Azure Active Directory Azure AD site tanımlayıcısını temsil eder."
type: docs
url: /tr/net/aspose.cells.metas/sensitivitylabel/siteid/
---
## SensitivityLabel.SiteId property

Hassasiyet etiketini tanımlayan hassasiyet etiketi politikasına karşılık gelen Azure Active Directory (Azure AD) site tanımlayıcısını temsil eder.

```csharp
public string SiteId { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertySiteIdDemo
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

                // İlk SiteId değerini almayı gösterin
                Console.WriteLine("Initial SiteId: " + label.SiteId);

                // SiteId'yi örnek bir Azure AD site tanımlayıcısı olarak ayarlayın
                label.SiteId = "a1b2c3d4-5678-90ef-ghij-klmnopqrstuv";
                Console.WriteLine("After setting SiteId: " + label.SiteId);

                // SiteId'yi değiştirerek okunabilir-yazılabilir olduğunu gösterin
                label.SiteId = "z9y8x7w6-5432-10uv-wxyz-abcdefghijkl";
                Console.WriteLine("Updated SiteId: " + label.SiteId);

                // SiteId'nin diğer özelliklerle nasıl ilişkili olduğunu gösterin
                Console.WriteLine($"Label {label.Id} with SiteId {label.SiteId} is enabled: {label.IsEnabled}");

                // Çalışma kitabını kaydedin
                workbook.Save("SiteIdDemo.xlsx");
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

* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


