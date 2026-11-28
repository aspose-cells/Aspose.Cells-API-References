---
title: "StyleFlag.TopBorder"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StyleFlag özelliği. Üst kenar ayarları uygulanacak"
type: docs
url: /tr/net/aspose.cells/styleflag/topborder/
---
## StyleFlag.TopBorder property

Üst kenar ayarları uygulanacak.

```csharp
public bool TopBorder { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyTopBorderDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Üst kenar ayarlarıyla bir stil oluşturun
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].Color = Color.Red;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Dashed;

            // Stil bayrağı oluşturun ve üst kenar değişikliğini etkinleştirin
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.TopBorder = true;

            // Sadece üst kenar bayrağı etkinleştirilmiş şekilde stili A1 hücresine uygulayın
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Sample Text");
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


