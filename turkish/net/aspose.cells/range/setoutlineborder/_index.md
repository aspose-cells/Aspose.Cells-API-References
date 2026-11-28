---
title: "Range.SetOutlineBorder"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. Hücre aralığı etrafına dış kenar çerçevesi ayarlar"
type: docs
url: /tr/net/aspose.cells/range/setoutlineborder/
---
## SetOutlineBorder(BorderType, CellBorderType, CellsColor) {#setoutlineborder}

Hücre aralığının etrafına dış kenarlık ayarlar.

```csharp
public void SetOutlineBorder(BorderType borderEdge, CellBorderType borderStyle, 
    CellsColor borderColor)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| borderEdge | BorderType | Kenarlık kenarı. |
| borderStyle | CellBorderType | Kenarlık stili. |
| borderColor | CellsColor | Kenarlık rengi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodSetOutlineBorderWithBorderTypeCellBorderTypeCellsCDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Bir CellsColor nesnesi oluştur
            CellsColor color = workbook.CreateCellsColor();
            color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            // Bir aralık oluştur ve sağ kenarlığı ayarla
            Aspose.Cells.Range range = cells.CreateRange("A2:B3");
            range.SetOutlineBorder(BorderType.RightBorder, CellBorderType.Thin, color);

            // Başka bir aralık oluştur ve tüm kenarlıkları ayarla
            range = cells.CreateRange("C6:F10");
            range.SetOutlineBorders(CellBorderType.Thin, color);

            // Çalışma kitabını kaydedin
            workbook.Save("SetOutlineBorderExample.xlsx");
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

---

## SetOutlineBorder(BorderType, CellBorderType, Color) {#setoutlineborder_1}

Hücre aralığının etrafına dış kenarlık ayarlar.

```csharp
public void SetOutlineBorder(BorderType borderEdge, CellBorderType borderStyle, Color borderColor)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| borderEdge | BorderType | Kenarlık kenarı. |
| borderStyle | CellBorderType | Kenarlık stili. |
| borderColor | Color | Kenarlık rengi. |

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodSetOutlineBorderWithBorderTypeCellBorderTypeColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir hücre aralığı oluşturun
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:D5");

            // Farklı kenarlık tipleri ve renkleriyle dış kenarlıkları ayarla
            range.SetOutlineBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Red);
            range.SetOutlineBorder(BorderType.RightBorder, CellBorderType.Medium, Color.Blue);
            range.SetOutlineBorder(BorderType.TopBorder, CellBorderType.Dashed, Color.Green);
            range.SetOutlineBorder(BorderType.BottomBorder, CellBorderType.Double, Color.Black);

            // Çalışma kitabını kaydedin
            workbook.Save("RangeOutlineBorderDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


