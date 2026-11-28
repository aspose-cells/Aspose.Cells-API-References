---
title: "SettableGlobalizationSettings.SetListSeparator"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableGlobalizationSettings yöntemi. Fonksiyonun liste parametreleri için ayırıcıyı ayarlar ...etc"
type: docs
url: /tr/net/aspose.cells/settableglobalizationsettings/setlistseparator/
---
## SettableGlobalizationSettings.SetListSeparator method

Liste, işlev parametreleri vb. için ayırıcıyı ayarlar.

```csharp
public void SetListSeparator(char c)
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

    public class SettableGlobalizationSettingsMethodSetListSeparatorWithCharDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özel küreselleşme ayarları oluşturun
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            try
            {
                // SetListSeparator yöntemini bir karakter parametresiyle çağırın
                settings.SetListSeparator(';');
                
                // Ayarları çalışma kitabına uygula
                workbook.Settings.GlobalizationSettings = settings;
                
                // Liste ayırıcı ile bir formül oluşturarak etkiyi gösterin
                worksheet.Cells["A1"].Formula = "SUM(1;2;3)";
                worksheet.Cells["A2"].Value = "Formula using custom list separator: SUM(1;2;3)";
                
                Console.WriteLine("SetListSeparator method executed successfully with parameter ';'");
                Console.WriteLine("Formula using custom list separator created in cell A1");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetListSeparator method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("SetListSeparatorWithCharDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


