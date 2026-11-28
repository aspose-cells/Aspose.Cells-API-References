---
title: "Range.SetOutlineBorders"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. Hücre aralığının etrafına aynı kenarlık stili ve rengiyle dış kenarlıklar ayarlar"
type: docs
url: /tr/net/aspose.cells/range/setoutlineborders/
---
## SetOutlineBorders(CellBorderType, CellsColor) {#setoutlineborders}

Hücre aralığının etrafındaki dış kenarlıkları aynı kenarlık stili ve rengiyle ayarlar.

```csharp
public void SetOutlineBorders(CellBorderType borderStyle, CellsColor borderColor)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| borderStyle | CellBorderType | Kenarlık stili. |
| borderColor | CellsColor | Kenarlık rengi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodSetOutlineBordersWithCellBorderTypeCellsColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Tema rengiyle bir CellsColor nesnesi oluştur
            CellsColor color = workbook.CreateCellsColor();
            color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            // Bir aralık oluştur ve dış kenarlıkları ayarla
            Aspose.Cells.Range range = cells.CreateRange("B2:D5");
            range.SetOutlineBorders(CellBorderType.Thin, color);

            // Çalışma kitabını kaydedin
            workbook.Save("OutlineBordersDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorders(CellBorderType, Color) {#setoutlineborders_1}

Hücre aralığının etrafındaki dış kenarlıkları aynı kenarlık stili ve rengiyle ayarlar.

```csharp
public void SetOutlineBorders(CellBorderType borderStyle, Color borderColor)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| borderStyle | CellBorderType | Kenarlık stili. |
| borderColor | Color | Kenarlık rengi. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System.Drawing;

    public class RangeMethodSetOutlineBordersWithCellBorderTypeColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1:D4 hücre aralığını oluştur
            Range range = worksheet.Cells.CreateRange("A1", "D4");

            // Kenarlıkları görünür kılmak için aralığı bazı verilerle doldur
            for (int row = 0; row < 4; row++)
            {
                for (int col = 0; col < 4; col++)
                {
                    worksheet.Cells[row, col].Value = $"Cell {row + 1},{col + 1}";
                }
            }

            try
            {
                // Orta kenarlık stili ve kırmızı renk ile SetOutlineBorders metodunu çağır
                range.SetOutlineBorders(CellBorderType.Medium, Color.Red);

                // Etkiyi görmek için çalışma kitabını kaydet
                workbook.Save("RangeMethodSetOutlineBordersWithCellBorderTypeColorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetOutlineBorders method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorders(CellBorderType[], Color[]) {#setoutlineborders_2}

Hücre aralığının etrafına dış kenarlıklar ayarlar.

```csharp
public void SetOutlineBorders(CellBorderType[] borderStyles, Color[] borderColors)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| borderStyles | CellBorderType[] | Kenarlık stilleri. |
| borderColors | Color[] | Kenarlık renkleri. |

### Açıklamalar

borderStyles ve borderStyles uzunlukları 4 olmalıdır. borderStyles sırası üst,alt,sol,sağ olmalıdır.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System.Drawing;

    public class RangeMethodSetOutlineBordersWithCellBorderTypeColorDemo1
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // B2:D4 hücre aralığını oluştur
            Range range = worksheet.Cells.CreateRange("B2", "D4");

            // Kenarlık stillerini ve renklerini hazırla
            CellBorderType[] borderStyles = new CellBorderType[]
            {
                CellBorderType.Thick,
                CellBorderType.Dashed,
                CellBorderType.Double,
                CellBorderType.MediumDashDot
            };

            Color[] borderColors = new Color[]
            {
                Color.Red,
                Color.Blue,
                Color.Green,
                Color.Purple
            };

            try
            {
                // Farklı stiller ve renklerle dış kenarlıkları ayarla
                range.SetOutlineBorders(borderStyles, borderColors);

                // Kenarlıkları görünür kılmak için hücreleri veriyle doldur
                for (int row = 1; row <= 3; row++)
                {
                    for (int col = 1; col <= 3; col++)
                    {
                        worksheet.Cells[row, col].PutValue($"Cell {row},{col}");
                    }
                }

                // Çalışma kitabını kaydedin
                workbook.Save("RangeSetOutlineBordersDemo.xlsx");
            }
            catch (System.Exception ex)
            {
                System.Console.WriteLine($"Error executing SetOutlineBorders method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


