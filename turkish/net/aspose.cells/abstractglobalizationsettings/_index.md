---
title: "Sınıf AbstractGlobalizationSettings"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.AbstractGlobalizationSettings sınıfı. Küreselleştirme ayarlarını temsil eder"
type: docs
url: /tr/net/aspose.cells/abstractglobalizationsettings/
---
## AbstractGlobalizationSettings class

Küreselleştirme ayarlarını temsil eder.

```csharp
public abstract class AbstractGlobalizationSettings
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| virtual [Compare](../../aspose.cells/abstractglobalizationsettings/compare/)(string, string, bool) | İki dize değerini belirli karşılaştırma kurallarına göre karşılaştırır. |
| virtual [GetCollationKey](../../aspose.cells/abstractglobalizationsettings/getcollationkey/)(string, bool) | Dizeyi belirli karşılaştırma kurallarına göre karşılaştırılabilir bir nesneye dönüştürür. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassAbstractGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // AbstractGlobalizationSettings'in özel bir uygulamasını oluşturun
            var customSettings = new CustomGlobalizationSettings();

            try
            {
                // Compare yöntemini gösterin
                string str1 = "Hello";
                string str2 = "hello";
                bool ignoreCase = true;

                int comparisonResult = customSettings.Compare(str1, str2, ignoreCase);
                Console.WriteLine($"Comparison result ({str1} vs {str2}, ignoreCase={ignoreCase}): {comparisonResult}");

                // GetCollationKey yöntemini gösterin
                string testString = "Sample";
                IComparable collationKey = customSettings.GetCollationKey(testString, ignoreCase);
                Console.WriteLine($"Collation key for '{testString}' (ignoreCase={ignoreCase}): {collationKey}");

                // Ayarları bir çalışma kitabına uygulayın
                Workbook workbook = new Workbook();
                workbook.Settings.GlobalizationSettings = customSettings;

                // Ayarların çalışmasını göstermek için bazı veriler ekleyin
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Apple");
                worksheet.Cells["A2"].PutValue("banana");
                worksheet.Cells["A3"].PutValue("Cherry");

                // Çalışma kitabını kaydedin
                workbook.Save("GlobalizationSettingsDemo.xlsx");
                Console.WriteLine("Workbook saved with custom globalization settings.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override int Compare(string v1, string v2, bool ignoreCase)
            {
                return string.Compare(v1, v2, ignoreCase ? StringComparison.OrdinalIgnoreCase : StringComparison.Ordinal);
            }

            public override IComparable GetCollationKey(string v, bool ignoreCase)
            {
                return ignoreCase ? v.ToLowerInvariant() : v;
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


