---
title: "AutoFilter.AddFontColorFilter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoFilter yöntemi. Bir yazı tipi renk filtresi ekler"
type: docs
url: /tr/net/aspose.cells/autofilter/addfontcolorfilter/
---
## AutoFilter.AddFontColorFilter method

Yazı tipi rengi filtresi ekler.

```csharp
public void AddFontColorFilter(int fieldIndex, CellsColor color)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | Int32 | Filtreyi temellendirmek istediğiniz alanın tam sayı ofseti (listenin solundan; en soldaki alan field 0'dır). |
| color | CellsColor | Bu [`CellsColor`](../../cellscolor/) nesnesi. |

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodAddFontColorFilterWithInt32CellsColorDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Farklı yazı tipi renkleriyle örnek veri ekle
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Item 1");
            cells["A3"].PutValue("Item 2");
            cells["A4"].PutValue("Item 3");
            
            // Yazı tipi renklerini ayarla
            Style style = cells["A2"].GetStyle();
            style.Font.Color = Color.Red;
            cells["A2"].SetStyle(style);
            
            style = cells["A3"].GetStyle();
            style.Font.Color = Color.Blue;
            cells["A3"].SetStyle(style);
            
            style = cells["A4"].GetStyle();
            style.Font.Color = Color.Green;
            cells["A4"].SetStyle(style);

            // Otomatik filtre uygula
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Kırmızı yazı tipi için renk filtresi oluştur
            CellsColor cr = workbook.CreateCellsColor();
            cr.Color = Color.Red;
            
            // Yazı tipi renk filtresi ekle
            filter.AddFontColorFilter(0, cr);
            filter.Refresh();
            
            // Çalışma kitabını kaydedin
            workbook.Save("AutoFilterFontColorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsColor](../../cellscolor/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


