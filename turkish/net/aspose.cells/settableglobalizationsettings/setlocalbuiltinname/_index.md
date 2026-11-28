---
title: "SettableGlobalizationSettings.SetLocalBuiltInName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableGlobalizationSettings yöntemi. Verilen standart ad metniyle yerel bağımlı yerleşik ad metnini ayarlar"
type: docs
url: /tr/net/aspose.cells/settableglobalizationsettings/setlocalbuiltinname/
---
## SettableGlobalizationSettings.SetLocalBuiltInName method

Verilen standart ad metniyle yerleşik ad için yerel bağımlı metni ayarlar.

```csharp
public void SetLocalBuiltInName(string standardName, string localName, bool bidirectional)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| standardName | String | Yerleşik adın standart (en-US yereli) ad metni. |
| localName | String | Yerel bağımlı ad metni |
| bidirectional | Boolean | Yerel ad metninin standart ad metnine otomatik olarak eşlenip eşlenmeyeceği. Doğru ise, yerel ad metni otomatik olarak standart ad metnine eşlenecek, böylece kullanıcı aynı standart ve yerel ad çifti için tekrar [`SetStandardBuiltInName`](../setstandardbuiltinname/) çağırmak zorunda kalmayacak |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetLocalBuiltInNameWithStringStringBooleanDemo
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
                // Standart bir yerleşik adı yerel bir ada eşlemek için SetLocalBuiltInName'i çağır
                settings.SetLocalBuiltInName("SUM", "LOCAL_SUM", true);

                // Ayarları çalışma kitabına uygula
                workbook.Settings.GlobalizationSettings = settings;

                // Standart yerleşik adı kullanarak bir formül oluştur
                worksheet.Cells["A1"].Formula = "=SUM(B1:B3)";
                worksheet.Cells["B1"].Value = 5;
                worksheet.Cells["B2"].Value = 10;
                worksheet.Cells["B3"].Value = 15;

                // Formülü hesapla
                workbook.CalculateFormula();

                Console.WriteLine("Formula with standard built-in name 'SUM' calculated successfully.");
                Console.WriteLine($"Result: {worksheet.Cells["A1"].Value}");

                // Yerel ad eşlemesini doğrula
                string localName = settings.GetLocalBuiltInName("SUM");
                Console.WriteLine($"Local name for 'SUM': {localName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLocalBuiltInName method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("SetLocalBuiltInNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


