---
title: "Enum DataBarAxisPosition"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.DataBarAxisPosition enum. Koşullu biçimlendirme ile veri çubukları olarak bir hücre aralığının eksen konumunu belirtir"
type: docs
url: /tr/net/aspose.cells/databaraxisposition/
---
## DataBarAxisPosition enumeration

Koşullu biçimlendirmeli hücre aralığı için veri çubukları olarak eksen konumunu belirtir.

```csharp
public enum DataBarAxisPosition
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Automatic | `0` | Eksen, aralıktaki minimum negatif değer ile maksimum pozitif değer oranına göre değişken bir konumda gösterilir. Pozitif değerler soldan sağa yönünde gösterilir. Negatif değerler sağdan sola yönünde gösterilir. Tüm değerler pozitif ya da tüm değerler negatif olduğunda eksen gösterilmez. |
| Midpoint | `1` | Eksen, aralıktaki değer kümesinden bağımsız olarak hücrenin orta noktasında gösterilir. Pozitif değerler soldan sağa yönünde gösterilir. Negatif değerler sağdan sola yönünde gösterilir. |
| None | `2` | Eksen gösterilmez ve hem pozitif hem negatif değerler soldan sağa yönünde gösterilir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarAxisPositionDemo
    {
        public static void DataBarAxisPositionExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();
            
            // Çalışma kitabındaki ilk çalışma sayfasına erişme
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Koşullu biçimlendirme kuralı ekleme
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Koşullu biçimlendirme aralığını ayarlama
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);
            
            // Veri çubuğu koşulu ekleme
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];
            DataBar dataBar = fc.DataBar;
            
            // Veri çubuğu için özellikleri ayarlama
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 30;
            dataBar.ShowValue = false;
            dataBar.BarBorder.Type = DataBarBorderType.Solid;
            dataBar.BarBorder.Color = Color.Plum;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint; // Using DataBarAxisPosition enum
            dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.Color = Color.White;
            dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.BorderColor = Color.Yellow;
            
            // Hücre değerlerini yerleştirme
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(120);
            worksheet.Cells["A3"].PutValue(260);
            
            // Excel dosyasını kaydetme
            workbook.Save("DataBarAxisPositionExample.xlsx");
            workbook.Save("DataBarAxisPositionExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


