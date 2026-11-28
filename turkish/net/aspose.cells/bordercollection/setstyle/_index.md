---
title: "BorderCollection.SetStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "BorderCollection yöntemi. Koleksiyonun tüm kenarlıklarının stilini ayarlar"
type: docs
url: /tr/net/aspose.cells/bordercollection/setstyle/
---
## BorderCollection.SetStyle method

Koleksiyondaki tüm kenarlıkların stilini ayarlar.

```csharp
public void SetStyle(CellBorderType style)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stil | CellBorderType | Kenarlıkların stili |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderCollectionMethodSetStyleWithCellBorderTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // C6 hücresini ve stilini al
            Cell cell = worksheet.Cells["C6"];
            Style style = cell.GetStyle();

            // Kenarlık rengini ve stilini ayarla
            style.Borders.SetColor(System.Drawing.Color.Red);
            style.Borders.SetStyle(CellBorderType.Thick);

            // Stili hücreye uygulayın
            cell.SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("BorderCollectionMethodSetStyleWithCellBorderTypeDemo_out.xlsx");

            Console.WriteLine("Border style set successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* enum [CellBorderType](../../cellbordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


