---
title: "SettableGlobalizationSettings.SetBooleanValueString"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableGlobalizationSettings yöntemi. Hücrelerin boolean değerinin görüntüleme dizesini ayarlar"
type: docs
url: /tr/net/aspose.cells/settableglobalizationsettings/setbooleanvaluestring/
---
## SettableGlobalizationSettings.SetBooleanValueString method

Hücrenin boolean değerinin görüntüleme dizesi değerini ayarlar

```csharp
public void SetBooleanValueString(bool bv, string name)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bv | Boolean | boolean değeri |
| name | String | boolean değerinin dize değeri |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetBooleanValueStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özel küreselleşme ayarları oluşturun
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Özel boolean değer dizesini ayarla
            settings.SetBooleanValueString(true, "Yes");
            settings.SetBooleanValueString(false, "No");
            
            // Ayarları çalışma kitabına uygula
            workbook.Settings.GlobalizationSettings = settings;
            
            // Hücrelerde boolean değerlerini ayarla
            worksheet.Cells["A1"].PutValue(true);
            worksheet.Cells["A2"].PutValue(false);
            
            // Boolean değerlerini metin olarak göstermek için görüntüleme stilini ayarla
            Style style = workbook.CreateStyle();
            style.Custom = "BOOLEAN";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A2"].SetStyle(style);
            
            try
            {
                // Çalışma kitabını kaydedin
                workbook.Save("SetBooleanValueStringDemo.xlsx");
                Console.WriteLine("Workbook saved with custom boolean value strings.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


