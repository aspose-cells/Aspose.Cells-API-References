---
title: "SettableGlobalizationSettings.GetStandardBuiltInName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableGlobalizationSettings yöntemi. Verilen yerel bağımlı metne göre yerleşik Name'in standart metnini alır"
type: docs
url: /tr/net/aspose.cells/settableglobalizationsettings/getstandardbuiltinname/
---
## SettableGlobalizationSettings.GetStandardBuiltInName method

Verilen yerel ayara bağlı metne göre yerleşik Name'in standart metnini alır.

```csharp
public override string GetStandardBuiltInName(string localName)
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

    public class SettableGlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // SettableGlobalizationSettings örneği oluştur
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            // Demonstrasyon için yerel bir yerleşik ad ayarlayın
            globalizationSettings.SetLocalBuiltInName("SUM", "LocalSumName", true);

            try
            {
                // Yerel bir adla GetStandardBuiltInName yöntemini çağırın
                string standardName = globalizationSettings.GetStandardBuiltInName("LocalSumName");
                
                // Sonucu göster
                Console.WriteLine($"Standard name for 'LocalSumName' is: {standardName}");

                // Sonucu bir hücreye uygulayın
                worksheet.Cells["A1"].Formula = "=" + standardName + "(1,2,3)";
                workbook.CalculateFormula();

                // Hesaplanan sonucu gösterin
                Console.WriteLine($"Result of formula in A1: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardBuiltInName method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("SettableGlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


