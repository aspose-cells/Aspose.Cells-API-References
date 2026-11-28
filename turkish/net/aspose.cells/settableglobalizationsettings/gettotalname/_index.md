---
title: "SettableGlobalizationSettings.GetTotalName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableGlobalizationSettings yöntemi. Belirli bir işlevin toplam adını alır"
type: docs
url: /tr/net/aspose.cells/settableglobalizationsettings/gettotalname/
---
## SettableGlobalizationSettings.GetTotalName method

Belirli işlevin toplam adını alır.

```csharp
public override string GetTotalName(ConsolidationFunction functionType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| functionType | ConsolidationFunction | İşlev tipi. |

### Dönüş Değeri

İşlevin toplam adı.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetTotalNameWithConsolidationFunctionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // SettableGlobalizationSettings örneği oluştur
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // GetTotalName'i ConsolidationFunction.Sum ile çağır
                string totalName = globalizationSettings.GetTotalName(ConsolidationFunction.Sum);
                
                // Sonucu göster
                Console.WriteLine($"Total name for Sum function: {totalName}");

                // Etkiyi göstermek için veri ekle (GetTotalName elektronik tabloyu değiştirmez)
                worksheet.Cells["A1"].PutValue("Values");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["B1"].PutValue("Total");
                worksheet.Cells["B4"].Formula = "=SUM(A2:A4)";
                
                // Formülleri hesapla
                workbook.CalculateFormula();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTotalName method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("SettableGlobalizationSettingsMethodGetTotalNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


