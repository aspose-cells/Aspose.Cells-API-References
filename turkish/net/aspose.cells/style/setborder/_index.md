---
title: "Style.SetBorder"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style yöntemi. Stilin kenarlarını ayarlar"
type: docs
url: /tr/net/aspose.cells/style/setborder/
---
## SetBorder(BorderType, CellBorderType, Color) {#setborder_1}

Stilin kenarlarını ayarlar.

```csharp
public bool SetBorder(BorderType borderType, CellBorderType borderStyle, Color borderColor)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| borderType | BorderType | Ayarlanacak kenar(lar), [`BorderType`](../../bordertype/) kombinasyonu olabilir. |
| borderStyle | CellBorderType | Kenarın stili. |
| borderColor | Color | Kenarlığın rengi. |

### Dönüş Değeri

Mevcut kenarlık ayarlarının değişip değişmediği.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleMethodSetBorderWithBorderTypeCellBorderTypeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            var range = worksheet.Cells.CreateRange("A1:D4");

            Style style = workbook.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.DiagonalDown, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.DiagonalUp, CellBorderType.Thin, Color.Blue);

            StyleFlag flag = new StyleFlag { Borders = true };
            range.ApplyStyle(style, flag);

            workbook.Save("BorderExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetBorder(BorderType, CellBorderType, CellsColor) {#setborder}

Stilin kenarlarını ayarlar.

```csharp
public bool SetBorder(BorderType borderType, CellBorderType borderStyle, CellsColor borderColor)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| borderType | BorderType | Ayarlanacak kenar(lar), [`BorderType`](../../bordertype/) kombinasyonu olabilir. |
| borderStyle | CellBorderType | Kenarın stili. |
| borderColor | CellsColor | Kenarlığın rengi. |

### Dönüş Değeri

Mevcut kenarlık ayarlarının değişip değişmediği.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleMethodSetBorderWithBorderTypeCellBorderTypeCellsCDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bağlam için bazı veriler ekle
            worksheet.Cells["A1"].Value = "Border Demo";
            
            try
            {
                // Bir stil oluştur
                Style style = workbook.CreateStyle();
                
                // Uygun fabrika yöntemi kullanarak bir CellsColor nesnesi oluştur
                CellsColor borderColor = workbook.CreateCellsColor();
                borderColor.Color = Color.Green;
                
                // SetBorder metodunu BorderType, CellBorderType ve CellsColor parametreleriyle çağır
                bool result = style.SetBorder(
                    BorderType.TopBorder, 
                    CellBorderType.Thick, 
                    borderColor);
                
                // Stili bir hücreye uygula
                worksheet.Cells["A1"].SetStyle(style);
                
                Console.WriteLine("SetBorder method called successfully. Result: " + result);
                
                // Çalışma kitabını kaydedin
                workbook.Save("SetBorderDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetBorder: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


