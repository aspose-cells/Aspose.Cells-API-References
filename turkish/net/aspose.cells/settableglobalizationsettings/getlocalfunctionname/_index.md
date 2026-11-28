---
title: "SettableGlobalizationSettings.GetLocalFunctionName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableGlobalizationSettings yöntemi. Verilen standart işlev adına göre yerel bağımlı işlev adını alır"
type: docs
url: /tr/net/aspose.cells/settableglobalizationsettings/getlocalfunctionname/
---
## SettableGlobalizationSettings.GetLocalFunctionName method

Verilen standart fonksiyon adına göre yerel ayara bağlı fonksiyon adını alır.

```csharp
public override string GetLocalFunctionName(string standardName)
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

    public class SettableGlobalizationSettingsMethodGetLocalFunctionNameWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özel küreselleşme ayarları oluşturun
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // "SUM" için özel bir yerel işlev adı ayarlayın
            settings.SetLocalFunctionName("SUM", "SOMME", true);

            // Ayarları çalışma kitabına uygula
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Yerelleştirilmiş adı almak için GetLocalFunctionName'ı çağırın
                string localName = settings.GetLocalFunctionName("SUM");
                
                // Sonucu göster
                Console.WriteLine($"Localized function name for 'SUM': {localName}");

                // Yerelleştirilmiş işlevi bir hücrede kullanın
                worksheet.Cells["A1"].Formula = "=SOMME(B1:B5)";
                worksheet.Cells["B1"].PutValue(1);
                worksheet.Cells["B2"].PutValue(2);
                worksheet.Cells["B3"].PutValue(3);
                worksheet.Cells["B4"].PutValue(4);
                worksheet.Cells["B5"].PutValue(5);

                // Formülleri hesapla
                workbook.CalculateFormula();

                // Sonucu göster
                Console.WriteLine($"Calculation result with localized function: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLocalFunctionName method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("MethodGetLocalFunctionNameWithStringDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


