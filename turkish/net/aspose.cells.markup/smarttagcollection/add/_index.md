---
title: "SmartTagCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SmartTagCollection yöntemi. Bir akıllı etiket ekler"
type: docs
url: /tr/net/aspose.cells.markup/smarttagcollection/add/
---
## SmartTagCollection.Add method

Bir akıllı etiket ekler.

```csharp
public int Add(string uri, string name)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uri | String | Akıllı etiketin ad alanı URI'sini belirtir |
| name | String | Akıllı etiketin adını belirtir. |

### Dönüş Değeri

Listede smart tag'in dizini.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagCollectionMethodAddWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            smartTagSetting.Add(0, 0); // Add smart tag to cell A1

            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
            int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            Console.WriteLine("Added smart tag at index: " + tagIndex);
            workbook.Save("SmartTagCollectionAddExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


