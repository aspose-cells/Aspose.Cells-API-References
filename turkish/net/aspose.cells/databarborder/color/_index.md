---
title: "DataBarBorder.Color"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataBarBorder özelliği. Koşullu biçimlendirme kuralı tarafından belirtilen veri çubuklarının kenar rengini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/databarborder/color/
---
## DataBarBorder.Color property

Koşullu biçimlendirme kuralı tarafından belirtilen veri çubuklarının kenarlık rengini alır veya ayarlar.

```csharp
public Color Color { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarBorderPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Biçim koşulu koleksiyonu oluştur
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            conds.AddArea(new CellArea { StartRow = 2, StartColumn = 4, EndRow = 3, EndColumn = 6 });

            // Veri çubuğu biçim koşulu ekle
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];

            // Veri çubuğu özelliklerini ayarla
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            cond.DataBar.ShowValue = false;

            // Kenarlık özelliklerini ayarla (Color kullanımını göstererek)
            cond.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            cond.DataBar.BarBorder.Color = Color.Plum;

            // Çalışma kitabını kaydedin
            workbook.Save("DataBarBorderColorDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("DataBar border color demo completed.");
        }
    }
}
```

### Ayrıca Bakınız

* class [DataBarBorder](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


