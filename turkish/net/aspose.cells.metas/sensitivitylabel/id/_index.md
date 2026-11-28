---
title: "SensitivityLabel.Id"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SensitivityLabel özelliği. Duyarlılık etiketinin kimliğini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.metas/sensitivitylabel/id/
---
## SensitivityLabel.Id property

Hassasiyet etiketinin kimliğini alır ve ayarlar.

```csharp
public string Id { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyIdDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // Bir duyarlılık etiketi örneği oluşturun
                Type labelType = typeof(SensitivityLabel);
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(labelType);
                
                // Id özelliğini ayarlamayı ve almayı gösterin
                string testId = "CONFIDENTIAL_001";
                label.Id = testId;
                
                // Id değerini gösterin
                Console.WriteLine("Sensitivity Label Id: " + label.Id);
                
                // Id değerini değiştirerek okunabilir-yazılabilir olduğunu gösterin
                label.Id = "INTERNAL_USE_ONLY";
                Console.WriteLine("Updated Sensitivity Label Id: " + label.Id);
                
                // Özelliğin diğer işlemleri etkilediğini gösterin
                label.IsEnabled = true;
                Console.WriteLine($"Label {label.Id} is enabled: {label.IsEnabled}");
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


