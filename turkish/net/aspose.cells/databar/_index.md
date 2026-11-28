---
title: "Class DataBar"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.DataBar sınıfı. DataBar koşullu biçimlendirme kuralını açıklar. Bu koşullu biçimlendirme kuralı, hücre aralığında dereceli bir veri çubuğu gösterir."
type: docs
url: /tr/net/aspose.cells/databar/
---
## DataBar class

DataBar koşullu biçimlendirme kuralını açıklayın. Bu koşullu biçimlendirme kuralı hücre aralığında kademeli bir veri çubuğu gösterir.

```csharp
public class DataBar
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AxisColor](../../aspose.cells/databar/axiscolor/) { get; set; } | Koşullu biçimlendirme veri çubukları olarak ayarlanmış hücrelerin eksen rengini alır. |
| [AxisPosition](../../aspose.cells/databar/axisposition/) { get; set; } | Koşullu biçimlendirme kuralı tarafından belirtilen veri çubuklarının eksen konumunu alır veya ayarlar. |
| [BarBorder](../../aspose.cells/databar/barborder/) { get; } | Bir veri çubuğunun kenarlığını belirten nesneyi alır. |
| [BarFillType](../../aspose.cells/databar/barfilltype/) { get; set; } | Bir veri çubuğunun renkle nasıl doldurulacağını alır veya ayarlar. |
| [Color](../../aspose.cells/databar/color/) { get; set; } | Bu DataBar'ın rengini al veya ayarla. |
| [Direction](../../aspose.cells/databar/direction/) { get; set; } | DataBar'ın görüntülendiği yönü alır veya ayarlar. |
| [MaxCfvo](../../aspose.cells/databar/maxcfvo/) { get; } | Bu DataBar'ın maksimum değer nesnesini al veya ayarla. Null veya FormatConditionValueType.Min tipinde CFValueObject'i ona atayamazsınız. |
| [MaxLength](../../aspose.cells/databar/maxlength/) { get; set; } | Veri çubuğunun maksimum uzunluğunu temsil eder. |
| [MinCfvo](../../aspose.cells/databar/mincfvo/) { get; } | Bu DataBar'ın minimum değer nesnesini al veya ayarla. Null veya FormatConditionValueType.Max tipinde CFValueObject'i ona atayamazsınız. |
| [MinLength](../../aspose.cells/databar/minlength/) { get; set; } | Veri çubuğunun minimum uzunluğunu temsil eder. |
| [NegativeBarFormat](../../aspose.cells/databar/negativebarformat/) { get; } | Bir veri çubuğu koşullu biçimlendirme kuralıyla ilişkili NegativeBarFormat nesnesini alır. |
| [ShowValue](../../aspose.cells/databar/showvalue/) { get; set; } | Bu veri çubuğunun uygulandığı hücrelerin değerlerinin gösterilip gösterilmeyeceğini belirten bayrağı al veya ayarla. Varsayılan değer doğrudur. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [ToImage](../../aspose.cells/databar/toimage/)(Cell, ImageOrPrintOptions) | Veri çubuğunu hücrede görüntü bayt dizisine dönüştürür. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarDemo
    {
        public static void DataBarExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Boş bir koşullu biçimlendirme ekler
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Koşullu biçimlendirme aralığını ayarlar
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Koşul ekler
            int idx = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = fcs[idx];

            // DataBar'ı al
            DataBar dataBar = cond.DataBar;

            // DataBar özelliklerini ayarla
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 30;
            dataBar.ShowValue = false;
            dataBar.BarBorder.Type = DataBarBorderType.Solid;
            dataBar.BarBorder.Color = Color.Plum;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint;
            dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.Color = Color.White;
            dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Hücre değerlerini yerleştir
            Aspose.Cells.Cell cell1 = sheet.Cells["A1"];
            cell1.PutValue(10);
            Aspose.Cells.Cell cell2 = sheet.Cells["A2"];
            cell2.PutValue(120);
            Aspose.Cells.Cell cell3 = sheet.Cells["A3"];
            cell3.PutValue(260);

            // Excel dosyasını kaydetme
            workbook.Save("DataBarExample.xlsx");
            workbook.Save("DataBarExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


