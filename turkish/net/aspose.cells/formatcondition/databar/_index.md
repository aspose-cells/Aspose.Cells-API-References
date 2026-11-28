---
title: "FormatCondition.DataBar"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormatCondition özelliği. Koşullu biçimlendirmelerin DataBar örneğini al. Varsayılan örnek rengi mavidir. Yalnızca DataBar türü için geçerlidir."
type: docs
url: /tr/net/aspose.cells/formatcondition/databar/
---
## FormatCondition.DataBar property

Koşullu biçimlendirme'nin "DataBar" örneğini al. Varsayılan örneğin rengi mavidir. Yalnızca type = DataBar için geçerlidir.

```csharp
public DataBar DataBar { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyDataBarDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // Veri çubuğu koşullu biçimlendirmesi ekle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Koşullu biçimlendirme için aralığı ayarla
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Veri çubuğu koşulunu ekle ve özellikleri ayarla
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = fcs[conditionIndex];
            
            // DataBar özelliklerini yapılandır
            DataBar dataBar = condition.DataBar;
            dataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            dataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            dataBar.Color = System.Drawing.Color.Green;

            // Çalışma kitabını kaydedin
            workbook.Save("DataBarExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DataBar](../../databar/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


