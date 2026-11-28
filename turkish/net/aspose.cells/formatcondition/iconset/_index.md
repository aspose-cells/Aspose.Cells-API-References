---
title: "FormatCondition.IconSet"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormatCondition özelliği. Koşullu biçimlendirmelerin IconSet örneğini alın. Varsayılan örnek IconSetType TrafficLights31'dir. Yalnızca IconSet türü için geçerlidir"
type: docs
url: /tr/net/aspose.cells/formatcondition/iconset/
---
## FormatCondition.IconSet property

Koşullu biçimlendirme'nin "IconSet" örneğini al. Varsayılan örneğin IconSetType'ı TrafficLights31'dir. Yalnızca type = IconSet için geçerlidir.

```csharp
public IconSet IconSet { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyIconSetDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i * 10);
            }

            // Koşullu biçimlendirme ekle
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            
            // Hücre aralığını ayarla
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Koşul ekle ve türü IconSet olarak ayarla
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcs[conditionIndex];
            
            // IconSet'i al ve yapılandır
            IconSet iconSet = condition.IconSet;
            iconSet.Type = IconSetType.TrafficLights31;
            iconSet.ShowValue = true;
            iconSet.Reverse = false;

            // Çalışma kitabını kaydedin
            workbook.Save("IconSetDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [IconSet](../../iconset/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


