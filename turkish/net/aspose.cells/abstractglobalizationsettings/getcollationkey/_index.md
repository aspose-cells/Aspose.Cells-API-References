---
title: "AbstractGlobalizationSettings.GetCollationKey"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AbstractGlobalizationSettings yöntemi. Belirli sıralama kurallarına göre dizeyi karşılaştırılabilir bir nesneye dönüştürür"
type: docs
url: /tr/net/aspose.cells/abstractglobalizationsettings/getcollationkey/
---
## AbstractGlobalizationSettings.GetCollationKey method

Dizeyi belirli karşılaştırma kurallarına göre karşılaştırılabilir bir nesneye dönüştürür.

```csharp
public virtual IComparable GetCollationKey(string v, bool ignoreCase)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| v | String | Dize değeri diğerleriyle karşılaştırılmalıdır. |
| ignoreCase | Boolean | değerleri karşılaştırırken büyük/küçük harf duyarsız olup olmayacağı |

### Dönüş Değeri

Nesne, dize değerlerini karşılaştırmak veya sıralamak için kullanılabilir

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractGlobalizationSettingsMethodGetCollationKeyWithStringBooleanDemo
    {
        public static void Run()
        {
            // GetCollationKey yöntemini geçersiz kılan özel küreselleştirme ayarları oluştur
            var settings = new CustomGlobalizationSettings();
            
            // Özel küreselleştirme ayarlarıyla bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = settings;

            // Sıralama anahtarı için dizeyi hazırla
            string inputString = "Sample Text";
            bool ignoreCase = true;

            try
            {
                // GetCollationKey'i doğrudan çağır
                IComparable collationKey = settings.GetCollationKey(inputString, ignoreCase);
                
                Console.WriteLine($"Original string: {inputString}");
                Console.WriteLine($"Collation key: {collationKey}");
                Console.WriteLine($"Ignore case: {ignoreCase}");

                // Çalışma sayfası işlemlerinde kullanarak etkiyi göster
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Apple");
                worksheet.Cells["A2"].PutValue("banana");
                worksheet.Cells["A3"].PutValue("Cherry");

                // Sıralama, GetCollationKey'i dahili olarak kullanacak
                DataSorter sorter = workbook.DataSorter;
                sorter.AddKey(0, SortOrder.Descending);

                sorter.Sort(worksheet.Cells, 0, 0, 2, 0);
                
                workbook.Save("GetCollationKeyDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during GetCollationKey operation: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override IComparable GetCollationKey(string v, bool ignoreCase)
            {
                return ignoreCase ? v.ToLowerInvariant() : v;
            }
        }

    }
}
```

### Ayrıca Bakınız

* class [AbstractGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


