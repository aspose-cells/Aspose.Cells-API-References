---
title: "SmartTagSetting.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SmartTagSetting yöntemi. Bir hücreye SmartTagCollection nesnesi ekler"
type: docs
url: /tr/net/aspose.cells.markup/smarttagsetting/add/
---
## Add(int, int) {#add}

Bir hücreye [`SmartTagCollection`](../../smarttagcollection/) nesnesi ekler.

```csharp
public int Add(int row, int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Hücrenin satırı. |
| sütun | Int32 | Hücrenin sütunu. |

### Dönüş Değeri

Çalışma sayfasında bir [`SmartTagCollection`](../../smarttagcollection/) nesnesinin dizinini döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagSettingMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0); // Add to cell A1 (row 0, column 0)

            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
            smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            Console.WriteLine("Smart Tags Count: " + smartTagSetting.Count.ToString());
            workbook.Save("SmartTagDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

Bir hücreye akıllı etiket ekle.

```csharp
public int Add(string cellName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | String | Hücrenin adı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagSettingMethodAddWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // SmartTagSetting örneğini al
            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            
            try
            {
                // String parametresiyle Add yöntemini çağır
                int index = smartTagSetting.Add("A1");
                
                Console.WriteLine($"SmartTag added successfully at index: {index}");
                
                // Etkiyi göstermek için bazı içerikler ekle
                worksheet.Cells["A1"].PutValue("This cell has a smart tag");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("SmartTagSettingMethodAddWithStringDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


