---
title: "StyleFlag.BottomBorder"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StyleFlag özelliği. Alt kenar ayarları uygulanacak"
type: docs
url: /tr/net/aspose.cells/styleflag/bottomborder/
---
## StyleFlag.BottomBorder property

Alt kenar ayarları uygulanacak.

```csharp
public bool BottomBorder { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyBottomBorderDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Alt kenar ayarlarıyla bir stil oluşturun
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.BottomBorder].Color = Color.Red;

            // Stil bayrağı oluşturun ve alt kenar değişikliğini etkinleştirin
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.BottomBorder = true;

            // Stili bayrakla birlikte A1 hücresine uygulayın
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Cell with bottom border");
            cell.SetStyle(style, styleFlag);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


