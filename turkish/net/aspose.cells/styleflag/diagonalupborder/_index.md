---
title: "StyleFlag.DiagonalUpBorder"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StyleFlag özelliği. Çapraz yukarı kenar ayarları uygulanacak"
type: docs
url: /tr/net/aspose.cells/styleflag/diagonalupborder/
---
## StyleFlag.DiagonalUpBorder property

Çapraz yukarı kenar ayarları uygulanacak.

```csharp
public bool DiagonalUpBorder { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleFlagPropertyDiagonalUpBorderDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine erişin ve bazı metinler ayarlayın
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Bir stil nesnesi oluşturun ve çapraz yukarı kenarı ayarlayın
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.DiagonalUp].Color = Color.FromArgb(255, 0, 0, 255);

            // Bir stil bayrağı oluşturun ve çapraz yukarı kenar bayrağını etkinleştirin
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.DiagonalUpBorder = true;

            // Bayrakla stili hücreye uygulayın
            cell.SetStyle(style, styleFlag);

            // Etkisini göstermek için başka bir hücre oluşturun
            Cell cell2 = worksheet.Cells["B2"];
            cell2.PutValue("Diagonal Up Border Demo");

            // Karşılaştırma için farklı bir stil oluşturun
            Style style2 = workbook.CreateStyle();
            style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.DiagonalUp].Color = Color.FromArgb(255, 0, 255, 0);

            // İkinci stili aynı bayrakla uygulayın
            cell2.SetStyle(style2, styleFlag);

            // Çalışma kitabını kaydedin
            workbook.Save("StyleFlagPropertyDiagonalUpBorderDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


