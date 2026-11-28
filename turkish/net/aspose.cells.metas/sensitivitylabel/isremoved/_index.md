---
title: "SensitivityLabel.IsRemoved"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SensitivityLabel özelliği. Hassasiyet etiketinin kaldırılıp kaldırılmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.metas/sensitivitylabel/isremoved/
---
## SensitivityLabel.IsRemoved property

Hassasiyet etiketinin kaldırılıp kaldırılmadığını gösterir.

```csharp
public bool IsRemoved { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyIsRemovedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // Yansıma (reflection) yoluyla bir hassasiyet etiketi örneği oluşturun
                // doğrudan örnekleme mümkün olmadığından
                Type labelType = typeof(SensitivityLabel);
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(labelType);
                
                // Gerekli özellikleri ayarlayın
                label.Id = "SENSITIVE_DATA";
                label.IsEnabled = true;
                label.IsRemoved = false;
                
                // İlk IsRemoved değerini gösterin
                Console.WriteLine("Initial IsRemoved value: " + label.IsRemoved);
                
                // IsRemoved özelliğini ayarlamayı gösterin (çünkü okunabilir-yazılabilir)
                label.IsRemoved = true;
                Console.WriteLine("After setting IsRemoved: " + label.IsRemoved);
                
                // Değeri geri değiştirerek değiştirilebileceğini gösterin
                label.IsRemoved = false;
                Console.WriteLine("Final IsRemoved value: " + label.IsRemoved);
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


