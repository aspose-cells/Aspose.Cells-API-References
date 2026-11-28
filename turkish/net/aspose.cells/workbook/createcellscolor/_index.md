---
title: "Workbook.CreateCellsColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Bir CellsColor nesnesi oluşturur"
type: docs
url: /tr/net/aspose.cells/workbook/createcellscolor/
---
## Workbook.CreateCellsColor method

Bir [`CellsColor`](../../cellscolor/) nesnesi oluşturur.

```csharp
public CellsColor CreateCellsColor()
```

### Dönüş Değeri

Bir [`CellsColor`](../../cellscolor/) nesnesi döndürür.

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateCellsColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Bir aralık oluşturun ve kenarlıkları özel renk ile ayarlayın
            Aspose.Cells.Range range = workbook.Worksheets[0].Cells.CreateRange("B5:F10");
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            range.SetInsideBorders(BorderType.Horizontal, CellBorderType.Thin, color);

            // Belirli bir hücrede kenarlık stilini doğrulayın
            Cell cell = workbook.Worksheets[0].Cells["F5"];
            Style style = cell.GetStyle();
            Console.WriteLine("Left Border: " + style.Borders[BorderType.LeftBorder].LineStyle);
            Console.WriteLine("Bottom Border: " + style.Borders[BorderType.BottomBorder].LineStyle);
            Console.WriteLine("Top Border: " + style.Borders[BorderType.TopBorder].LineStyle);
            Console.WriteLine("Right Border: " + style.Borders[BorderType.RightBorder].LineStyle);

            workbook.Save("CreateCellsColorExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsColor](../../cellscolor/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


