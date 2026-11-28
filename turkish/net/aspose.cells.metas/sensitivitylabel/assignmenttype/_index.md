---
title: "SensitivityLabel.AssignmentType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SensitivityLabel özelliği. Hassasiyet etiketi için atama yöntemini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.metas/sensitivitylabel/assignmenttype/
---
## SensitivityLabel.AssignmentType property

Hassasiyet etiketi için atama yöntemini alır ve ayarlar.

```csharp
public SensitivityLabelAssignmentType AssignmentType { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyAssignmentTypeDemo
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
                
                // İlk AssignmentType değerini almayı gösterin
                Console.WriteLine("Initial AssignmentType: " + label.AssignmentType);
                
                // AssignmentType'ı Privileged olarak ayarlayın ve değişikliği gösterin
                label.AssignmentType = SensitivityLabelAssignmentType.Privileged;
                Console.WriteLine("After setting Privileged: " + label.AssignmentType);
                
                // Okunabilir-yazılabilir olduğunu göstermek için Standard'a geri değiştirin
                label.AssignmentType = SensitivityLabelAssignmentType.Standard;
                Console.WriteLine("After setting Standard: " + label.AssignmentType);
                
                // Çalışma kitabını kaydedin
                workbook.Save("AssignmentTypeDemo.xlsx");
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

* enum [SensitivityLabelAssignmentType](../../sensitivitylabelassignmenttype/)
* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


