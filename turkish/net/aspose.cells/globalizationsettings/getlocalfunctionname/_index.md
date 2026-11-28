---
title: "GlobalizationSettings.GetLocalFunctionName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GlobalizationSettings yöntemi. Verilen standart fonksiyon adına göre yerel bağımlı fonksiyon adını alır"
type: docs
url: /tr/net/aspose.cells/globalizationsettings/getlocalfunctionname/
---
## GlobalizationSettings.GetLocalFunctionName method

Verilen standart fonksiyon adına göre yerel ayara bağlı fonksiyon adını alır.

```csharp
public virtual string GetLocalFunctionName(string standardName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| standardName | String | Standart (en-US yerel ayarı) fonksiyon adı. |

### Dönüş Değeri

Yerel ayara bağlı fonksiyon adı. Bu ayarların kullanıldığı Çalışma Kitabı tarafından yerel ayar belirtilmiştir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetLocalFunctionNameWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özel küreselleştirme ayarlarını ayarla
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            // Örnek veri ekleyin.
            worksheet.Cells["B1"].PutValue(5);
            worksheet.Cells["B2"].PutValue(15);

            // Yerelleştirilmiş fonksiyon adıyla formül oluştur
            Cell cell = worksheet.Cells["B3"];
            cell.Formula = "=LOCALSUM(B1:B2)";

            try
            {
                workbook.CalculateFormula();
                Console.WriteLine($"Calculation result using localized function: {cell.DoubleValue}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Calculation error: {ex.Message}");
            }

            workbook.Save("GlobalizationSettingsFunctionDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetLocalFunctionName(string standardName)
            {
                if (standardName == "SUM")
                {
                    return "LOCALSUM";
                }
                return base.GetLocalFunctionName(standardName);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


