---
title: "Class SensitivityLabel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Metas.SensitivityLabel class. Hassasiyet etiketini temsil eder"
type: docs
url: /tr/net/aspose.cells.metas/sensitivitylabel/
---
## SensitivityLabel class

Hassasiyet etiketini temsil eder.

```csharp
public class SensitivityLabel
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AssignmentType](../../aspose.cells.metas/sensitivitylabel/assignmenttype/) { get; set; } | Hassasiyet etiketi için atama yöntemini alır ve ayarlar. |
| [ContentMarkType](../../aspose.cells.metas/sensitivitylabel/contentmarktype/) { get; set; } | Bir dosyaya uygulanması gereken içerik işaretleme türlerini alır ve ayarlar. |
| [Id](../../aspose.cells.metas/sensitivitylabel/id/) { get; set; } | Hassasiyet etiketinin kimliğini alır ve ayarlar. |
| [IsEnabled](../../aspose.cells.metas/sensitivitylabel/isenabled/) { get; set; } | Hassasiyet etiketinin etkin olup olmadığını gösterir |
| [IsRemoved](../../aspose.cells.metas/sensitivitylabel/isremoved/) { get; set; } | Hassasiyet etiketinin kaldırılıp kaldırılmadığını gösterir. |
| [SiteId](../../aspose.cells.metas/sensitivitylabel/siteid/) { get; set; } | Hassasiyet etiketini tanımlayan hassasiyet etiketi politikasına karşılık gelen Azure Active Directory (Azure AD) site tanımlayıcısını temsil eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class MetasClassSensitivityLabelDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // Reflection kullanarak SensitivityLabel sınıfının bir örneğini oluşturun
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // Temel özellikleri ayarlayın
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;
                label.AssignmentType = SensitivityLabelAssignmentType.Standard;
                label.ContentMarkType = SensitivityLabelMarkType.None;
                
                // Özellik değerlerini göster
                Console.WriteLine($"Sensitivity Label Created:");
                Console.WriteLine($"ID: {label.Id}");
                Console.WriteLine($"Enabled: {label.IsEnabled}");
                Console.WriteLine($"Assignment Type: {label.AssignmentType}");
                Console.WriteLine($"Content Mark Type: {label.ContentMarkType}");
                
                // Çalışma kitabını kaydedin
                workbook.Save("SensitivityLabelDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SensitivityLabel: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)


