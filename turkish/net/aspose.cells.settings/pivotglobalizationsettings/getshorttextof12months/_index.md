---
title: "PivotGlobalizationSettings.GetShortTextOf12Months"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotGlobalizationSettings yöntemi. 12 ayın tüm kısa biçimlendirilmiş dizesini alır"
type: docs
url: /tr/net/aspose.cells.settings/pivotglobalizationsettings/getshorttextof12months/
---
## PivotGlobalizationSettings.GetShortTextOf12Months method

12 ayın tüm kısa biçimli dizesini alır.

```csharp
public virtual string[] GetShortTextOf12Months()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Settings;
    using System;

    public class PivotGlobalizationSettingsMethodGetShortTextOf12MonthsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // PivotGlobalizationSettings sınıfından türeten özel bir küreselleştirme ayarları sınıfı oluşturun
            var customGlobalizationSettings = new CustomPivotGlobalizationSettings();

            try
            {
                // GetShortTextOf12Months yöntemini çağırın
                string[] monthShortNames = customGlobalizationSettings.GetShortTextOf12Months();

                // Ay adlarını konsola çıktı olarak verin
                Console.WriteLine("Short names of 12 months:");
                foreach (string monthName in monthShortNames)
                {
                    Console.WriteLine(monthName);
                }

                // Ay adlarını çalışma sayfasına ekleyin
                for (int i = 0; i < monthShortNames.Length; i++)
                {
                    worksheet.Cells[i, 0].PutValue(monthShortNames[i]);
                }

                Console.WriteLine("Method executed successfully. Month names added to worksheet.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetShortTextOf12Months method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("MethodGetShortTextOf12MonthsDemo.xlsx");
        }
    }

    // GetShortTextOf12Months yöntemini geçersiz kılmak için PivotGlobalizationSettings'in özel uygulaması
    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string[] GetShortTextOf12Months()
        {
            // Özel kısa ay adlarını döndürün
            return new string[] { "Jan", "Feb", "Mar", "Apr", "May", "Jun", 
                                "Jul", "Aug", "Sep", "Oct", "Nov", "Dec" };
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


