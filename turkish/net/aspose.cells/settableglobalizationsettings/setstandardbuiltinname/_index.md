---
title: "SettableGlobalizationSettings.SetStandardBuiltInName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableGlobalizationSettings yöntemi. Verilen standart işlev adına göre yerel bağımlı işlev adını ayarlar"
type: docs
url: /tr/net/aspose.cells/settableglobalizationsettings/setstandardbuiltinname/
---
## SettableGlobalizationSettings.SetStandardBuiltInName method

Verilen standart işlev adına göre yerel bağımlı işlev adını ayarlar.

```csharp
public void SetStandardBuiltInName(string localName, string standardName, bool bidirectional)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| localName | String | Yerel bağımlı işlev adı |
| standardName | String | Standart (en-US yerel ayarı) fonksiyon adı. |
| bidirectional | Boolean | Standart ad metnini yerel ad metnine otomatik olarak eşleyip eşlemeyeceğini belirler. Doğru ise, standart ad metni otomatik olarak yerel ad metnine eşlenecek, böylece kullanıcı aynı standart ve yerel ad çifti için tekrar [`SetLocalBuiltInName`](../setlocalbuiltinname/) çağırmak zorunda kalmayacak. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardBuiltInNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Özel küreselleşme ayarları oluşturun
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Çalışma kitabı için küreselleştirme ayarlarını ayarlayın
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Yerel bir adı standart yerleşik bir ada eşlemek için SetStandardBuiltInName'i çağırın
                // Parametreler: localName, standardName, bidirectional
                settings.SetStandardBuiltInName("MyLocalName", "SUM", true);
                
                Console.WriteLine("SetStandardBuiltInName executed successfully with parameters (\"MyLocalName\", \"SUM\", true)");
                
                // Yerel adı bir formülde kullanarak etkiyi gösterin
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["A3"].Formula = "=MyLocalName(A1:A2)";
                
                // Formülü hesaplayarak yerel adla çalıştığını gösterin
                workbook.CalculateFormula();
                Console.WriteLine("Result of formula with local name: " + worksheet.Cells["A3"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardBuiltInName method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("SetStandardBuiltInNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


