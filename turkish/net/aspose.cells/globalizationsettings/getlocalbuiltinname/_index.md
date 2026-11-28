---
title: "GlobalizationSettings.GetLocalBuiltInName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GlobalizationSettings yöntemi. Verilen standart metne göre yerel bağımlı yerleşik Name metnini alır"
type: docs
url: /tr/net/aspose.cells/globalizationsettings/getlocalbuiltinname/
---
## GlobalizationSettings.GetLocalBuiltInName method

Verilen standart metne göre yerel ayara bağlı yerleşik Name metnini alır.

```csharp
public virtual string GetLocalBuiltInName(string standardName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| standardName | String | Yerleşik Name'in Standart (en-US yereli) metni. |

### Dönüş Değeri

Yerel bağımlı metin. Yerel, bu ayarların kullanıldığı Workbook tarafından belirtilmiştir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetLocalBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                string standardName = "Total";
                string localizedName = ((CustomGlobalizationSettings)workbook.Settings.GlobalizationSettings).GetLocalBuiltInName(standardName);

                Console.WriteLine($"Standard Name: {standardName}");
                Console.WriteLine($"Localized Name: {localizedName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLocalBuiltInName method: {ex.Message}");
            }

            workbook.Save("LocalizedBuiltInNameDemo.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetLocalBuiltInName(string standardName)
        {
            switch (standardName)
            {
                case "Total":
                    return "LocalizedTotal";
                case "Average":
                    return "LocalizedAverage";
                default:
                    return base.GetLocalBuiltInName(standardName);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


