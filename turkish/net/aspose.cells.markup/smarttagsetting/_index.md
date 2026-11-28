---
title: "Sınıf SmartTagSetting"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Markup.SmartTagSetting sınıfı. Çalışma sayfasındaki tüm SmartTagCollection nesnelerini temsil eder"
type: docs
url: /tr/net/aspose.cells.markup/smarttagsetting/
---
## SmartTagSetting class

Çalışma sayfasındaki tüm [`SmartTagCollection`](../smarttagcollection/) nesnelerini temsil eder.

```csharp
public class SmartTagSetting : CollectionBase
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Item](../../aspose.cells.markup/smarttagsetting/item/) { get; } | İndeksle bir [`SmartTagCollection`](../smarttagcollection/) nesnesi alır. (3 indeksleyici) |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells.markup/smarttagsetting/add/#add_1)(string) | Bir hücreye akıllı etiket ekle. |
| [Add](../../aspose.cells.markup/smarttagsetting/add/#add)(int, int) | Bir hücreye bir [`SmartTagCollection`](../smarttagcollection/) nesnesi ekler. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagSettingDemo
    {
        public static void SmartTagSettingExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Belirli bir hücreye akıllı etiket ekle
            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0); // Adding smart tag to cell A1

            // Hücre için SmartTagCollection'a erişin
            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];

            // Koleksiyona bir akıllı etiket ekleyin
            int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            // Akıllı etiket ayarının kapasitesini ayarlayın
            smartTagSetting.Capacity = 10;

            // Akıllı etiketlerin sayısını yazdırın
            Console.WriteLine("Total Smart Tags: " + smartTagSetting.Count);

            // Çalışma kitabını kaydedin
            workbook.Save("SmartTagSettingExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


