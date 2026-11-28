---
title: "GlobalizationSettings.GetBooleanValueString"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GlobalizationSettings yöntemi. Hücrelerin boolean değerleri için görüntüleme dizesi değerini alır"
type: docs
url: /tr/net/aspose.cells/globalizationsettings/getbooleanvaluestring/
---
## GlobalizationSettings.GetBooleanValueString method

Hücrenin boolean değerinin görüntüleme dizesi değerini alır

```csharp
public virtual string GetBooleanValueString(bool bv)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bv | Boolean | boolean değeri |

### Dönüş Değeri

Varsayılan olarak doğru değer için "TRUE", yanlış değer için "FALSE" döndürür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetBooleanValueStringWithBooleanDemo
    {
        public static void Run()
        {
            // Özel küreselleştirme ayarlarıyla yeni bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomBooleanGlobalizationSettings();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // GetBooleanValueString yöntemini her iki boolean değerle göster
                var globalizationSettings = workbook.Settings.GlobalizationSettings;
                string trueResult = globalizationSettings.GetBooleanValueString(true);
                string falseResult = globalizationSettings.GetBooleanValueString(false);

                Console.WriteLine($"GetBooleanValueString(true) returns: {trueResult}");
                Console.WriteLine($"GetBooleanValueString(false) returns: {falseResult}");

                // Hücrelere boolean değerler uygula ve elektronik tablo etkisini göster
                worksheet.Cells["A1"].PutValue(true);
                worksheet.Cells["A2"].PutValue(false);

                workbook.Save("GlobalizationBooleanDemo.xlsx");
                Console.WriteLine("Workbook saved with custom boolean representations.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBooleanValueString: {ex.Message}");
            }
        }
    }

    // Boolean dize temsilini geçersiz kılan özel küreselleştirme ayarları
    public class CustomBooleanGlobalizationSettings : GlobalizationSettings
    {
        public override string GetBooleanValueString(bool bv)
        {
            return bv ? "Enabled" : "Disabled";
        }
    }
}
```

### Ayrıca Bakınız

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


