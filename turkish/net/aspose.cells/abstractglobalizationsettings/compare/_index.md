---
title: "AbstractGlobalizationSettings.Compare"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AbstractGlobalizationSettings yöntemi. Belirli sıralama kurallarına göre iki dize değerini karşılaştırır"
type: docs
url: /tr/net/aspose.cells/abstractglobalizationsettings/compare/
---
## AbstractGlobalizationSettings.Compare method

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

    public class AbstractGlobalizationSettingsMethodCompareWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Compare yöntemini geçersiz kılan özel küreselleştirme ayarları oluştur
            var settings = new CustomGlobalizationSettings();
            
            // Özel küreselleştirme ayarlarıyla bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = settings;

            // Karşılaştırmak için dizeleri hazırla
            string string1 = "Apple";
            string string2 = "apple";
            bool ignoreCase = true;

            try
            {
                // Compare yöntemi, sıralama gibi işlemler sırasında dahili olarak çağrılacak
                // Burada doğrudan kullanımı gösteriyoruz
                int comparisonResult = settings.Compare(string1, string2, ignoreCase);
                
                Console.WriteLine($"Comparison result: {comparisonResult}");
                Console.WriteLine($"Strings compared: '{string1}' and '{string2}' (Ignore case: {ignoreCase})");

                // Verileri sıralayarak etkiyi göster
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Orange");
                worksheet.Cells["A2"].PutValue("apple");
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["A4"].PutValue("Apple");

                // Bir DataSorter oluştur ve sıralama aralığını ayarla
                DataSorter sorter = workbook.DataSorter;
                sorter.AddKey(0, SortOrder.Ascending);

                sorter.Sort(worksheet.Cells, 0, 0, 3, 0);
                workbook.Save("StringComparisonDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during string comparison: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override int Compare(string v1, string v2, bool ignoreCase)
            {
                return String.Compare(v1, v2, ignoreCase);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [AbstractGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


