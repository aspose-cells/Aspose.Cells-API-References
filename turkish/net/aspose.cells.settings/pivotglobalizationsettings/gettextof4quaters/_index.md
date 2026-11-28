---
title: "PivotGlobalizationSettings.GetTextOf4Quaters"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotGlobalizationSettings yöntemi. 4 çeyrek için yerel metni alır"
type: docs
url: /tr/net/aspose.cells.settings/pivotglobalizationsettings/gettextof4quaters/
---
## PivotGlobalizationSettings.GetTextOf4Quaters method

4 Çeyrek'in yerel metnini alır.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOf4Quarters() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string[] GetTextOf4Quaters()
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine, lütfen PivotGlobalizationSettings.GetTextOf4Quarters() yöntemini kullanın. Bu özellik Temmuz 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Settings;
    using System;

    public class PivotGlobalizationSettingsMethodGetTextOf4QuatersDemo
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
                // GetTextOf4Quaters yöntemini çağır
                string[] quarterNames = customGlobalizationSettings.GetTextOf4Quaters();

                // Çeyrek adlarını konsola çıktı olarak ver
                Console.WriteLine("Names of 4 quarters:");
                foreach (string quarterName in quarterNames)
                {
                    Console.WriteLine(quarterName);
                }

                // Çeyrek adlarını çalışma sayfasına ekle
                for (int i = 0; i < quarterNames.Length; i++)
                {
                    worksheet.Cells[i, 0].PutValue(quarterNames[i]);
                }

                Console.WriteLine("Method executed successfully. Quarter names added to worksheet.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTextOf4Quaters method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("MethodGetTextOf4QuatersDemo.xlsx");
        }
    }

    // GetTextOf4Quaters yöntemini geçersiz kılmak için PivotGlobalizationSettings'in özel uygulaması
    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string[] GetTextOf4Quaters()
        {
            // Özel çeyrek adlarını döndür
            return new string[] { "First Quarter", "Second Quarter", 
                               "Third Quarter", "Fourth Quarter" };
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


