---
title: "SmartTagPropertyCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SmartTagPropertyCollection yöntemi. Hücre akıllı etiketi özelliği ekler"
type: docs
url: /tr/net/aspose.cells.markup/smarttagpropertycollection/add/
---
## SmartTagPropertyCollection.Add method

Hücrenin akıllı etiketine bir özellik ekler.

```csharp
public int Add(string name, string value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Özelliğin adı |
| değer | String | Özelliğin değeri. |

### Dönüş Değeri

döndür [`SmartTagProperty`](../../smarttagproperty/)

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagPropertyCollectionMethodAddWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = sheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0);
            SmartTagCollection smartTags = smartTagSetting[smartTagIndex];

            smartTags.Add("http://docs.aspose.com", "docs");
            SmartTag smartTag = smartTags[0];

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

* class [SmartTagPropertyCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


