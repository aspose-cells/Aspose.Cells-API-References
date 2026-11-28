---
title: "AutoFilter.AddFillColorFilter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoFilter yöntemi. Dolgu rengi filtresi ekler"
type: docs
url: /tr/net/aspose.cells/autofilter/addfillcolorfilter/
---
## AutoFilter.AddFillColorFilter method

Dolgu rengi filtresi ekler.

```csharp
public void AddFillColorFilter(int fieldIndex, BackgroundType pattern, CellsColor foregroundColor, 
    CellsColor backgroundColor)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | Int32 | Filtreyi temellendirmek istediğiniz alanın tam sayı ofseti (listenin solundan; en soldaki alan field 0'dır). |
| desen | BackgroundType | Arka plan desen türü. |
| foregroundColor | CellsColor | Ön plan rengi. |
| backgroundColor | CellsColor | Arka plan rengi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodAddFillColorFilterWithInt32BackgroundTypeCellsColorCDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Farklı dolgu renkleriyle örnek veri ekle
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Data1");
            cells["A3"].PutValue("Data2");
            cells["A4"].PutValue("Data3");
            
            // Farklı dolgu renklerini uygula
            Style style1 = cells["A2"].GetStyle();
            style1.ForegroundColor = Color.Red;
            style1.Pattern = BackgroundType.Solid;
            cells["A2"].SetStyle(style1);
            
            Style style2 = cells["A3"].GetStyle();
            style2.ForegroundColor = Color.Blue;
            style2.Pattern = BackgroundType.Solid;
            cells["A3"].SetStyle(style2);
            
            Style style3 = cells["A4"].GetStyle();
            style3.ForegroundColor = Color.Green;
            style3.Pattern = BackgroundType.Solid;
            cells["A4"].SetStyle(style3);

            // Otomatik filtre oluştur
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Filtreleme için hücre renkleri oluştur
            CellsColor filterColor = workbook.CreateCellsColor();
            filterColor.Color = Color.Red;
            
            // Dolgu rengi filtresini uygula
            filter.AddFillColorFilter(0, BackgroundType.Solid, filterColor, filterColor);
            filter.Refresh();
            
            // Çalışma kitabını kaydedin
            workbook.Save("AutoFilterFillColorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [BackgroundType](../../backgroundtype/)
* class [CellsColor](../../cellscolor/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


