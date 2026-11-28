---
title: "SettableGlobalizationSettings.SetStandardFunctionName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableGlobalizationSettings yöntemi. Verilen standart işlev adına göre yerel bağımlı işlev adını ayarlar"
type: docs
url: /tr/net/aspose.cells/settableglobalizationsettings/setstandardfunctionname/
---
## SettableGlobalizationSettings.SetStandardFunctionName method

Verilen standart işlev adına göre yerel bağımlı işlev adını ayarlar.

```csharp
public void SetStandardFunctionName(string localName, string standardName, bool bidirectional)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| localName | String | Yerel bağımlı işlev adı |
| standardName | String | Standart (en-US yerel ayarı) fonksiyon adı. |
| bidirectional | Boolean | Standart işlev adının yerel işlev adına otomatik olarak eşlenip eşlenmeyeceği. Doğru ise, standart ad otomatik olarak yerel ada eşlenecek, böylece kullanıcı aynı standart ve yerel ad çifti için tekrar [`SetLocalFunctionName`](../setlocalfunctionname/) çağırmak zorunda kalmayacak |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardFunctionNameWithStringStringBooleanDemo
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
                // Yerel bir işlev adını standart ada eşlemek için SetStandardFunctionName'i çağır
                settings.SetStandardFunctionName("LOCAL_SUM", "SUM", true);

                // Ayarları çalışma kitabına uygula
                workbook.Settings.GlobalizationSettings = settings;

                // Yerel işlev adını kullanarak bir formül oluştur
                worksheet.Cells["A1"].Formula = "=LOCAL_SUM(B1:B3)";
                worksheet.Cells["B1"].Value = 10;
                worksheet.Cells["B2"].Value = 20;
                worksheet.Cells["B3"].Value = 30;

                // Formülü hesapla
                workbook.CalculateFormula();

                Console.WriteLine("Formula with local function name 'LOCAL_SUM' calculated successfully.");
                Console.WriteLine($"Result: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardFunctionName method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("SetStandardFunctionNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


