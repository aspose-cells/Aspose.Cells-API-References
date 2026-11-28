---
title: "Range.SetStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range metodu. Hücre stilini uygulayın"
type: docs
url: /tr/net/aspose.cells/range/setstyle/
---
## SetStyle(Style, bool) {#setstyle_1}

Hücre stilini uygula.

```csharp
public void SetStyle(Style style, bool explicitFlag)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stil | Stil | Hücre stili. |
| explicitFlag | Boolean | Doğru, yalnızca açıkça ayarlanmış biçimlendirmeyi üzerine yazar. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangeMethodSetStyleWithStyleBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Style style = wb.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;
            
            Aspose.Cells.Range range = wb.Worksheets[0].Cells.CreateRange(0, 0, 1, 5);
            range.SetStyle(style, true);
            
            wb.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style) {#setstyle}

Aralığın stilini ayarlar.

```csharp
public void SetStyle(Style style)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stil | Stil | Style nesnesi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangeMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir stil oluştur
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            style.Font.IsBold = true;
            style.Font.Color = Color.Red;
            style.Font.Underline = FontUnderlineType.Single;

            // Stili bir hücreye uygula
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["A1"].SetStyle(style);

            // Bir aralık oluşturun ve aynı stili uygulayın
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "C3");
            range.SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("RangeMethodSetStyleWithStyleDemo_output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


