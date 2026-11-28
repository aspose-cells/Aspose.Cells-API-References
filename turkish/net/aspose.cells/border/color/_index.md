---
title: "Border.Color"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Border özelliği. Kenarın rengini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/border/color/
---
## Border.Color property

Kenarlığın rengini alır veya ayarlar.

```csharp
public Color Color { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BorderPropertyColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1 hücresine eriş
            Cell cell = worksheet.Cells["A1"];
            
            // Hücre değerini ayarla
            cell.PutValue("Border Color Demo");
            
            // Hücrenin stilini al
            Style style = cell.GetStyle();
            
            // Kenarlık renklerini ve stillerini ayarla
            style.Borders[BorderType.TopBorder].Color = Color.Red;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            
            style.Borders[BorderType.BottomBorder].Color = Color.Blue;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dotted;
            
            style.Borders[BorderType.LeftBorder].Color = Color.Green;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dashed;
            
            style.Borders[BorderType.RightBorder].Color = Color.FromArgb(255, 128, 0); // Orange
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            
            // Stili hücreye uygulayın
            cell.SetStyle(style);
            
            // Çalışma kitabını kaydedin
            workbook.Save("BorderColorDemo.xlsx");
            
            Console.WriteLine("Border color demo created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


