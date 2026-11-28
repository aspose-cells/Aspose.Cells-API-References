---
title: "Sınıf BorderCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.BorderCollection sınıf. Border nesnelerinin bir koleksiyonunu kapsar"
type: docs
url: /tr/net/aspose.cells/bordercollection/
---
## BorderCollection class

[`Border`](../border/) nesnelerinin bir koleksiyonunu kapsar.

```csharp
public class BorderCollection
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [DiagonalColor](../../aspose.cells/bordercollection/diagonalcolor/) { get; set; } | Çapraz çizgilerin Rengini alır veya ayarlar. |
| [DiagonalStyle](../../aspose.cells/bordercollection/diagonalstyle/) { get; set; } | Çapraz çizgilerin stilini alır veya ayarlar. |
| [IsOutline](../../aspose.cells/bordercollection/isoutline/) { get; set; } | Bir hücre aralığının dış kenarlarına yalnızca uygulanması gerektiğini, sol, sağ, üst ve alt kenarlıkların gösterir. Varsayılan değer true'dur. |
| [Item](../../aspose.cells/bordercollection/item/) { get; } | Belirtilen indeksteki [`Border`](../border/) öğesini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [SetColor](../../aspose.cells/bordercollection/setcolor/)(Color) | Koleksiyondaki tüm kenarlıkların rengini ayarlar. |
| [SetStyle](../../aspose.cells/bordercollection/setstyle/)(CellBorderType) | Koleksiyondaki tüm kenarlıkların stilini ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BorderCollectionDemo
    {
        public static void BorderCollectionExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();

            // Workbook nesnesine yeni bir çalışma sayfası ekleme
            workbook.Worksheets.Add();

            // Eklenen yeni çalışma sayfasının referansını, sayfa indeksini geçirerek elde etme
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasından "A1" hücresine erişme
            Cell cell = worksheet.Cells["A1"];

            // "A1" hücresine bir değer ekleme
            cell.PutValue("Visit Aspose!");

            // Hücrenin stilini alma
            Style style = cell.GetStyle();

            // Üst kenarlığın çizgi stilini ayarlama
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;

            // Üst kenarlığın rengini ayarlama
            style.Borders[BorderType.TopBorder].Color = Color.Red;

            // Alt kenarlığın çizgi stilini ayarlama
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thick;

            // Alt kenarlığın rengini ayarlama
            style.Borders[BorderType.BottomBorder].Color = Color.Green;

            // Sol kenarlığın çizgi stilini ayarlama
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dashed;

            // Sol kenarlığın rengini ayarlama
            style.Borders[BorderType.LeftBorder].Color = Color.Yellow;

            // Sağ kenarlığın çizgi stilini ayarlama
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Dotted;

            // Sağ kenarlığın rengini ayarlama
            style.Borders[BorderType.RightBorder].Color = Color.Blue;

            // Çapraz özelliklerini ayarlama
            style.Borders.DiagonalColor = Color.Red;
            style.Borders.DiagonalStyle = CellBorderType.Dashed;

            // Stili hücreye uygulama
            cell.SetStyle(style);

            // Excel dosyasını kaydetme
            workbook.Save("BorderCollectionExample.xlsx");
            workbook.Save("BorderCollectionExample.pdf");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


