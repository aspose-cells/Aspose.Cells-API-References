---
title: "Range.SetInsideBorders"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. Aralığın iç kenarlarını ayarlar"
type: docs
url: /tr/net/aspose.cells/range/setinsideborders/
---
## Range.SetInsideBorders method

Aralığın iç kenarlıklarını ayarla.

```csharp
public void SetInsideBorders(BorderType borderEdge, CellBorderType lineStyle, 
    CellsColor borderColor)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| borderEdge | BorderType | İç kenar türü, yalnızca Dikey ve Yatay olabilir. |
| lineStyle | CellBorderType | Kenarlık stili. |
| borderColor | CellsColor | Kenarlığın rengi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangeMethodSetInsideBordersWithBorderTypeCellBorderTypeCellsCDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir aralık oluşturun ve iç kenarları ayarlayın
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B5:F10");
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            range.SetInsideBorders(BorderType.Vertical, CellBorderType.Thin, color);

            // Aralık içindeki bir hücredeki kenarları doğrulayın
            Cell cell = worksheet.Cells["C6"];
            Style style = cell.GetStyle();
            Console.WriteLine("Left Border: " + style.Borders[BorderType.LeftBorder].LineStyle);
            Console.WriteLine("Right Border: " + style.Borders[BorderType.RightBorder].LineStyle);
            Console.WriteLine("Top Border: " + style.Borders[BorderType.TopBorder].LineStyle);
            Console.WriteLine("Bottom Border: " + style.Borders[BorderType.BottomBorder].LineStyle);

            workbook.Save("SetInsideBordersExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


