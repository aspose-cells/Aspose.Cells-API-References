---
title: "SmartTagSetting.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SmartTagSetting özelliği. Dizine göre bir SmartTagCollection nesnesi alır"
type: docs
url: /tr/net/aspose.cells.markup/smarttagsetting/item/
---
## SmartTagSetting indexer (1 of 3)

Dizine göre bir [`SmartTagCollection`](../../smarttagcollection/) nesnesi alır.

```csharp
public SmartTagCollection this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| index | Listede [`SmartTagCollection`](../../smarttagcollection/) nesnesinin dizini. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagSettingPropertyItemDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Aspose");
            sheet.Cells["A2"].PutValue("Cells");

            SmartTagSetting smartTagSetting = sheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0);
            
            // Item özelliğinin kullanımını göster
            SmartTagCollection smartTags = smartTagSetting[smartTagIndex];
            smartTags.Add("http://docs.aspose.com", "docs");
            
            SmartTag smartTag = smartTags[0];
            smartTag.SetLink("http://www.aspose.com", "AsposeLink");

            SmartTagPropertyCollection properties = smartTag.Properties;
            properties.Add("Author", "Aspose");
            properties.Add("Version", "1.0");

            workbook.Save("SmartTagPropertyDemo.xlsx");
            Console.WriteLine("SmartTagPropertyDemo.xlsx created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagSetting indexer (2 of 3)

Hücrenin [`SmartTagCollection`](../../smarttagcollection/) nesnesini alır.

```csharp
public SmartTagCollection this[int row, int column] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| satır | Hücrenin satır indeksi. |
| sütun | Hücrenin sütun dizini |

### Dönüş Değeri

Hücrenin [`SmartTagCollection`](../../smarttagcollection/) nesnesini döndürür. Hücrede akıllı etiket yoksa null döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagSettingPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            smartTagSetting.Add(0, 0); // Add smart tag to cell A1

            // Item özelliğinin kullanımını göster
            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
            smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            Console.WriteLine("Smart tags in cell A1: " + smartTagCollection.Count);
            Console.WriteLine("Namespace URI: " + smartTagCollection[0].Uri);
            Console.WriteLine("Tag name: " + smartTagCollection[0].Name);

            workbook.Save("SmartTagDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagSetting indexer (3 of 3)

Hücrenin [`SmartTagCollection`](../../smarttagcollection/) nesnesini alır.

```csharp
public SmartTagCollection this[string cellName] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| cellName | Hücrenin adı. |

### Dönüş Değeri

Hücrenin [`SmartTagCollection`](../../smarttagcollection/) nesnesini döndürür. Hücrede akıllı etiket yoksa null döndürür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagSettingPropertyItemDemo2
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasını al
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Çalışma sayfası için SmartTagSetting'e eriş
                SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;

                // A1 hücresine (satır 0, sütun 0) bir akıllı etiket ekle
                int smartTagIndex = smartTagSetting.Add(0, 0);

                // Item özelliğinin kullanımını göster (indeksleyici)
                SmartTagCollection smartTagCollection = smartTagSetting[smartTagIndex];

                // Koleksiyona bir akıllı etiket ekleyin
                smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

                // Akıllı etiket hakkında bilgi göster
                Console.WriteLine("Number of smart tags in collection: " + smartTagCollection.Count);
                if (smartTagCollection.Count > 0)
                {
                    Console.WriteLine("First smart tag URI: " + smartTagCollection[0].Uri);
                    Console.WriteLine("First smart tag name: " + smartTagCollection[0].Name);
                }

                // Çalışma kitabını kaydedin
                workbook.Save("SmartTagItemDemo.xlsx");
                Console.WriteLine("SmartTagItemDemo.xlsx created successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


