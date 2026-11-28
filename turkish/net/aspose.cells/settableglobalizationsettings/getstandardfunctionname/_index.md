---
title: "SettableGlobalizationSettings.GetStandardFunctionName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableGlobalizationSettings yöntemi. Verilen yerel ayara bağlı fonksiyon adına göre standart fonksiyon adını alır"
type: docs
url: /tr/net/aspose.cells/settableglobalizationsettings/getstandardfunctionname/
---
## SettableGlobalizationSettings.GetStandardFunctionName method

Verilen yerel ayara bağlı fonksiyon adına göre standart fonksiyon adını alır.

```csharp
public override string GetStandardFunctionName(string localName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| localName | String | Yerel ayara bağlı fonksiyon adı. Bu ayarların kullanıldığı Çalışma Kitabı tarafından yerel ayar belirtilmiştir. |

### Dönüş Değeri

Standart (en-US yerel ayarı) fonksiyon adı.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özel küreselleşme ayarları oluşturun
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Yerel bir fonksiyon adı eşlemesi ayarla
            settings.SetStandardFunctionName("LocalSum", "SUM", true);

            // Ayarları çalışma kitabına uygula
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Yerel bir fonksiyon adıyla GetStandardFunctionName'i çağır
                string standardName = settings.GetStandardFunctionName("LocalSum");
                
                // Sonucu göster
                Console.WriteLine($"Standard function name for 'LocalSum' is: {standardName}");

                // Hücre formülünde standart fonksiyonu kullan
                worksheet.Cells["A1"].Formula = $"={standardName}(1,2,3)";
                worksheet.Cells["A2"].Value = 1;
                worksheet.Cells["A3"].Value = 2;
                worksheet.Cells["A4"].Value = 3;

                // Formülü hesapla
                workbook.CalculateFormula();

                // Sonucu göster
                Console.WriteLine($"Formula result in A1: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardFunctionName method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("SettableGlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


