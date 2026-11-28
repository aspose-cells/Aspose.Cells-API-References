---
title: "GlobalizationSettings.GetStandardFunctionName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GlobalizationSettings yöntemi. Verilen yerel bağımlı fonksiyon adına göre standart fonksiyon adını alır."
type: docs
url: /tr/net/aspose.cells/globalizationsettings/getstandardfunctionname/
---
## GlobalizationSettings.GetStandardFunctionName method

Verilen yerel ayara bağlı fonksiyon adına göre standart fonksiyon adını alır.

```csharp
public virtual string GetStandardFunctionName(string localName)
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

    public class GlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veriyi hazırlayın.
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(15);
            
            // Özel küreselleştirme ayarlarını oluşturun ve çalışma kitabına atayın.
            var customSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = customSettings;

            try
            {
                // Almanca SUM fonksiyon adıyla GetStandardFunctionName'i gösterin.
                string localName = "SUMME";
                string standardName = customSettings.GetStandardFunctionName(localName);
                
                Console.WriteLine($"Local function name: {localName}");
                Console.WriteLine($"Standard function name: {standardName}");

                // Formülde yerelleştirilmiş fonksiyon adını uygulayın.
                worksheet.Cells["A3"].Formula = "=SUMME(A1:A2)";
                workbook.CalculateFormula();
                
                Console.WriteLine($"Formula result: {worksheet.Cells["A3"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardFunctionName method: {ex.Message}");
            }

            workbook.Save("MethodGetStandardFunctionNameDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetStandardFunctionName(string localName)
            {
                // Almanca fonksiyon adını standart İngilizceye dönüştür.
                if (localName.Equals("SUMME", StringComparison.OrdinalIgnoreCase))
                {
                    return "SUM";
                }
                return base.GetStandardFunctionName(localName);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


