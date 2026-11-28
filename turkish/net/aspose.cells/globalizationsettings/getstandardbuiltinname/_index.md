---
title: "GlobalizationSettings.GetStandardBuiltInName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GlobalizationSettings yöntemi. Verilen yerel ayara bağlı metne göre yerleşik Name'in standart metnini alır"
type: docs
url: /tr/net/aspose.cells/globalizationsettings/getstandardbuiltinname/
---
## GlobalizationSettings.GetStandardBuiltInName method

Verilen yerel ayara bağlı metne göre yerleşik Name'in standart metnini alır.

```csharp
public virtual string GetStandardBuiltInName(string localName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| localName | String | Yerleşik Name'in yerel bağımlı metni. Yerel, bu ayarların kullanıldığı Workbook tarafından belirtilmiştir. |

### Dönüş Değeri

Standart (en-US yereli) metin.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // Özel küreselleştirme ayarlarıyla bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özel küreselleştirme ayarlarını başlat ve çalışma kitabına ata
            var globalizationSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = globalizationSettings;

            // GetStandardBuiltInName için test parametresi
            string localFunctionName = "MyLocalSum";
            
            try
            {
                // Yerel fonksiyon adıyla GetStandardBuiltInName'i çağır
                string standardName = globalizationSettings.GetStandardBuiltInName(localFunctionName);
                Console.WriteLine($"Local name: '{localFunctionName}' => Standard name: '{standardName}'");

                // Formülde yerel adı kullanarak etkiyi göster
                worksheet.Cells["A1"].Value = 5;
                worksheet.Cells["A2"].Value = 7;
                worksheet.Cells["A3"].Formula = $"{localFunctionName}(A1:A2)";

                // Doğru yorumlamayı göstermek için formülü hesapla
                workbook.CalculateFormula();
                Console.WriteLine($"Formula result: {worksheet.Cells["A3"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardBuiltInName: {ex.Message}");
            }

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("GlobalizationGetStandardBuiltInNameDemo.xlsx");
        }
    }

    // GetStandardBuiltInName'i geçersiz kılan özel küreselleştirme ayarları
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetStandardBuiltInName(string localName)
        {
            // Özel yerel fonksiyon adını standart SUM'a eşle
            if (localName.Equals("MyLocalSum", StringComparison.OrdinalIgnoreCase))
            {
                return "SUM";
            }
            return base.GetStandardBuiltInName(localName);
        }
    }
}
```

### Ayrıca Bakınız

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


