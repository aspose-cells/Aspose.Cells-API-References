---
title: "SensitivityLabel.IsEnabled"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SensitivityLabel özelliği. Hassasiyet etiketinin etkin olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.metas/sensitivitylabel/isenabled/
---
## SensitivityLabel.IsEnabled property

Hassasiyet etiketinin etkin olup olmadığını gösterir

```csharp
public bool IsEnabled { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyIsEnabledDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // Bir duyarlılık etiketi örneği oluşturun
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // İlk özellikleri ayarlayın
                label.Id = "CONFIDENTIAL_001";
                
                // İlk IsEnabled değerini almayı gösterin
                Console.WriteLine("Initial IsEnabled value: " + label.IsEnabled);
                
                // IsEnabled'ı true olarak ayarlayın ve değişikliği gösterin
                label.IsEnabled = true;
                Console.WriteLine("After enabling: " + label.IsEnabled);
                
                // Değeri değiştirerek okunabilir-yazılabilir olduğunu gösterin
                label.IsEnabled = false;
                Console.WriteLine("After disabling: " + label.IsEnabled);
                
                // Çalışma kitabını kaydedin
                workbook.Save("IsEnabledDemo.xlsx");
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


