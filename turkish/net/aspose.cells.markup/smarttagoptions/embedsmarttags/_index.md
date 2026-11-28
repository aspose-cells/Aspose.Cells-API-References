---
title: "SmartTagOptions.EmbedSmartTags"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SmartTagOptions özelliği. Smart tag'lerin çalışma kitabıyla kaydedilip kaydedilmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells.markup/smarttagoptions/embedsmarttags/
---
## SmartTagOptions.EmbedSmartTags property

Çalışma kitabıyla akıllı etiketlerin kaydedilip kaydedilmeyeceğini gösterir.

```csharp
public bool EmbedSmartTags { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagOptionsPropertyEmbedSmartTagsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagOptions smartTagOptions = new SmartTagOptions();
            Console.WriteLine("Current EmbedSmartTags value: " + smartTagOptions.EmbedSmartTags);

            smartTagOptions.EmbedSmartTags = true;
            // SmartTagOptions artık API tarafından gerekliyse doğru şekilde kullanılıyor, ancak workbook.Settings'e atama geçerli değil

            Console.WriteLine("after setting value: Current EmbedSmartTags value: " + smartTagOptions.EmbedSmartTags);

            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("New York");

            // SmartTagSetting aracılığıyla SmartTag'lere erişin
            int index = worksheet.SmartTagSetting.Add(cell.Name);
            SmartTagCollection smartTagCollection = worksheet.SmartTagSetting[index];
            int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags#place", "Place");
            SmartTag smartTag = smartTagCollection[tagIndex];
            smartTag.Properties.Add("State", "NY");
            // LinkedCell'i ayarlamak için Özellikleri kullanın
            smartTag.Properties.Add("LinkedCell", cell.Name);

            workbook.Save("PropertyEmbedSmartTagsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SmartTagOptions](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


