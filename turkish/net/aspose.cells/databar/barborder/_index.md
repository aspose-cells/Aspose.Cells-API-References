---
title: "DataBar.BarBorder"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataBar özelliği. Veri çubuğunun kenarlığını belirten bir nesne döndürür"
type: docs
url: /tr/net/aspose.cells/databar/barborder/
---
## DataBar.BarBorder property

Bir veri çubuğunun kenarlığını belirten nesneyi alır.

```csharp
public DataBarBorder BarBorder { get; }
```

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyBarBorderDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);

            // Veri çubuğu koşullu biçimlendirmesi ekle
            int idx = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[idx];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Veri çubuğu koşulu ekle
            int conditionIdx = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIdx];

            // Veri çubuğu özelliklerini ayarla
            fc.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            fc.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            fc.DataBar.Color = Color.Blue;
            fc.DataBar.ShowValue = true;

            // Çubuk kenarlık özelliklerini ayarla
            fc.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            fc.DataBar.BarBorder.Color = Color.Black;

            // Çalışma kitabını kaydedin
            workbook.Save("DataBarBorderDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DataBarBorder](../../databarborder/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


