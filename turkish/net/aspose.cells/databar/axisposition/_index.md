---
title: "DataBar.AxisPosition"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataBar özelliği. Koşullu biçimlendirme kuralı tarafından belirlenen veri çubuklarının eksen konumunu alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/databar/axisposition/
---
## DataBar.AxisPosition property

Koşullu biçimlendirme kuralı tarafından belirtilen veri çubuklarının eksen konumunu alır veya ayarlar.

```csharp
public DataBarAxisPosition AxisPosition { get; set; }
```

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyAxisPositionDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            sheet.Cells["E3"].PutValue(10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(30);
            sheet.Cells["F4"].PutValue(40);
            sheet.Cells["G3"].PutValue(-15);
            sheet.Cells["G4"].PutValue(-25);

            // Veri çubuğu koşullu biçimlendirmesi ekle
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];
            
            // Veri çubuğu özelliklerini yapılandır
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            cond.DataBar.ShowValue = false;
            
            // Eksen konumunu ayarla (temel gösterim)
            cond.DataBar.AxisPosition = DataBarAxisPosition.Automatic;
            cond.DataBar.AxisColor = Color.Red;

            // Çalışma kitabını kaydedin
            workbook.Save("DataBarAxisPositionDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("DataBar with AxisPosition demo created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* enum [DataBarAxisPosition](../../databaraxisposition/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


