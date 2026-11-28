---
title: "SettableGlobalizationSettings.SetLocalFunctionName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableGlobalizationSettings yöntemi. Verilen standart fonksiyon adına karşılık gelen yerel bağımlı fonksiyon adını ayarlar"
type: docs
url: /tr/net/aspose.cells/settableglobalizationsettings/setlocalfunctionname/
---
## SettableGlobalizationSettings.SetLocalFunctionName method

Verilen standart işlev adına karşılık gelen yerel bağımlı işlev adını ayarlar.

```csharp
public void SetLocalFunctionName(string standardName, string localName, bool bidirectional)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| standardName | String | Standart (en-US yerel ayarı) fonksiyon adı. |
| localName | String | Yerel bağımlı işlev adı |
| bidirectional | Boolean | Yerel fonksiyon adının standart fonksiyon adına otomatik olarak eşlenip eşlenmeyeceği. True ise, yerel ad otomatik olarak standart ada eşlenecek, böylece kullanıcı aynı standart ve yerel ad çifti için tekrar [`SetStandardFunctionName`](../setstandardfunctionname/) çağırmak zorunda kalmayacak |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetLocalFunctionNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Küreselleştirme ayarları oluştur
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // SetLocalFunctionName'i çağırarak standart fonksiyon adını yerel ada eşle
                settings.SetLocalFunctionName("SUM", "SOMMA", true); // Italian localization for SUM function
                settings.SetLocalFunctionName("AVERAGE", "MEDIA", true); // Italian localization for AVERAGE function

                // Ayarları çalışma kitabına uygula
                workbook.Settings.GlobalizationSettings = settings;

                // Hem standart hem de yerelleştirilmiş adları kullanan formüller oluştur
                worksheet.Cells["A1"].Formula = "=SUM(B1:B5)";
                worksheet.Cells["A2"].Formula = "=SOMMA(B1:B5)";
                worksheet.Cells["A3"].Formula = "=AVERAGE(B1:B5)";
                worksheet.Cells["A4"].Formula = "=MEDIA(B1:B5)";

                // Formülleri hesapla
                workbook.CalculateFormula();

                Console.WriteLine("SetLocalFunctionName executed successfully with parameters (String, String, Boolean)");
                Console.WriteLine("Standard and localized function names work equivalently in formulas.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLocalFunctionName method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("MethodSetLocalFunctionNameWithStringStringBooleanDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


