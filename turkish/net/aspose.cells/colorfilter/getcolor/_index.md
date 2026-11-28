---
title: "ColorFilter.GetColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ColorFilter yöntemi. Bu filtrenin rengini alır"
type: docs
url: /tr/net/aspose.cells/colorfilter/getcolor/
---
## ColorFilter.GetColor method

Bu filtrenin rengini alır.

```csharp
public Color GetColor(WorksheetCollection sheets)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sayfalar | WorksheetCollection |  |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ColorFilterMethodGetColorWithWorksheetCollectionDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["A4"].PutValue("Item 3");
            
            // Otomatik filtre oluştur
            worksheet.AutoFilter.Range = "A1:A4";
            
            // Renk filtresi oluşturun
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            worksheet.AutoFilter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
            worksheet.AutoFilter.Refresh();
            
            // Renk filtresini al ve rengini doğrula
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            ColorFilter colorFilter = filterColumn.Filter as ColorFilter;
            
            if (colorFilter != null)
            {
                Color retrievedColor = colorFilter.GetColor(workbook.Worksheets);
                Console.WriteLine("Filter color: " + retrievedColor.ToString());
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [WorksheetCollection](../../worksheetcollection/)
* class [ColorFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


