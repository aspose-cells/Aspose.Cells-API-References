---
title: "GlobalizationSettings.Compare"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GlobalizationSettings yöntemi. Belirli karşılaştırma kurallarına göre iki string değerini karşılaştırır"
type: docs
url: /tr/net/aspose.cells/globalizationsettings/compare/
---
## GlobalizationSettings.Compare method

İki dize değerini belirli karşılaştırma kurallarına göre karşılaştırır.

```csharp
public virtual int Compare(string v1, string v2, bool ignoreCase)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| v1 | String | ilk dize |
| v2 | String | ikinci dize |
| ignoreCase | Boolean | değerleri karşılaştırırken büyük/küçük harf duyarsız olup olmayacağı |

### Dönüş Değeri

İki karşılaştırılan öğe arasındaki sözcüksel ilişkiyi gösteren tam sayı

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodCompareWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Özel küreselleştirme ayarlarıyla bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomComparisonSettings();

            try
            {
                // Doğrudan Compare yöntemi kullanımını gösterin
                GlobalizationSettings settings = workbook.Settings.GlobalizationSettings;
                int result1 = settings.Compare("Apple", "apple", true);
                int result2 = settings.Compare("Apple", "apple", false);
                
                Console.WriteLine($"Case-insensitive comparison result: {result1}");
                Console.WriteLine($"Case-sensitive comparison result: {result2}");

                // Elektronik tablo işlemleri üzerindeki etkiyi gösterin
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Banana");
                worksheet.Cells["A2"].PutValue("apple");
                worksheet.Cells["A3"].PutValue("Cherry");

                // Özel karşılaştırma kullanarak verileri sırala
                DataSorter sorter = workbook.DataSorter;
                sorter.Order1 = SortOrder.Ascending;
                sorter.Key1 = 0;
                sorter.Sort(worksheet.Cells, 0, 0, 2, 0); // Corrected range to rows 0-2

                Console.WriteLine("Sorted data with custom comparison rules:");
                for (int row = 0; row < 3; row++)
                {
                    Cell cell = worksheet.Cells[row, 0];
                    Console.WriteLine(cell.StringValue);
                }

                workbook.Save("GlobalizationCompareDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomComparisonSettings : GlobalizationSettings
    {
        public override int Compare(string v1, string v2, bool ignoreCase)
        {
            // Özel karşılaştırma mantığını uygula
            var comparison = ignoreCase ? 
                StringComparison.OrdinalIgnoreCase : 
                StringComparison.Ordinal;
            
            return string.Compare(v1?.Trim() ?? "", v2?.Trim() ?? "", comparison);
        }
    }
}
```

### Ayrıca Bakınız

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


