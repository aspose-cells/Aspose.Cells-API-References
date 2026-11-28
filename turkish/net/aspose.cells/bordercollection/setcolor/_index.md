---
title: "BorderCollection.SetColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "BorderCollection yöntemi. Koleksiyondaki tüm kenarlıkların Renk değerini ayarlar"
type: docs
url: /tr/net/aspose.cells/bordercollection/setcolor/
---
## BorderCollection.SetColor method

Koleksiyondaki tüm kenarlıkların rengini ayarlar.

```csharp
public void SetColor(Color color)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| color | Color | Kenarlıkların Rengi. |

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderCollectionMethodSetColorWithColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Renkli kenarlara sahip bir stil oluşturun
            Style style = workbook.CreateStyle();
            
            // Kenarlık çizgi stillerini ayarlayın
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            // SetColor yöntemi kullanarak kenarlık rengini kırmızı olarak ayarlayın
            style.Borders.SetColor(Color.Red);

            // Stili bir hücreye uygula
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Cell with colored borders");
            cell.SetStyle(style);

            // Daha iyi görünürlük için sütunu otomatik sığdırın
            worksheet.AutoFitColumn(0);

            // Çalışma kitabını kaydedin
            workbook.Save("BorderColorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


