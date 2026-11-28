---
title: "SettableGlobalizationSettings.SetRowSeparatorOfFormulaArray"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableGlobalizationSettings yöntemi. Formüldeki dizi verisinin satırları için ayırıcıyı ayarlar"
type: docs
url: /tr/net/aspose.cells/settableglobalizationsettings/setrowseparatorofformulaarray/
---
## SettableGlobalizationSettings.SetRowSeparatorOfFormulaArray method

Formülde dizi verisindeki satırlar için ayırıcıyı ayarlar.

```csharp
public void SetRowSeparatorOfFormulaArray(char c)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| c | Char | belirtilen ayırıcı |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetRowSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özel küreselleşme ayarları oluşturun
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Formül dizileri için satır ayırıcıyı '|' olarak ayarla
            char rowSeparator = '|';
            settings.SetRowSeparatorOfFormulaArray(rowSeparator);

            // Ayarları çalışma kitabına uygula
            workbook.Settings.GlobalizationSettings = settings;

            // Çalışma sayfasında bir dizi formülü oluştur
            worksheet.Cells["A1"].SetArrayFormula("={1,2,3;4,5,6}", 2, 3);
            
            try
            {
                // Ayarları uygulamak için formülü hesapla
                workbook.CalculateFormula();

                // Yeni satır ayırıcıyla formülü göster
                Console.WriteLine("Array formula with custom row separator: " + worksheet.Cells["A1"].Formula);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetRowSeparatorOfFormulaArray method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("MethodSetRowSeparatorOfFormulaArrayDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


