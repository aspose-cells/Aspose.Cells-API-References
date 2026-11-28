---
title: "CellsColor.ColorIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsColor özelliği. Renk paletindeki renk indeksini alır ve ayarlar. Yalnızca indeksli renklere uygulanır"
type: docs
url: /tr/net/aspose.cells/cellscolor/colorindex/
---
## CellsColor.ColorIndex property

Renk paletindeki renk indeksini alır ve ayarlar. Yalnızca indeksli renkler için geçerlidir.

```csharp
public int ColorIndex { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;

    public class CellsColorPropertyColorIndexDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Renkli bir kenarlık uygulayacağımız bir aralık tanımlayın
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:D4");

            // Bir CellsColor örneği oluştur
            CellsColor cellsColor = workbook.CreateCellsColor();

            // ColorIndex'i (palet indeksi) ayarlayın – örneğin, 5
            cellsColor.ColorIndex = 5;

            // CellsColor'i aralığın iç kenarlık rengi olarak uygulayın
            range.SetInsideBorders(BorderType.Horizontal | BorderType.Vertical,
                                   CellBorderType.Thin,
                                   cellsColor);

            // Mevcut ColorIndex değerini okuyun ve görüntüleyin
            Console.WriteLine("Current ColorIndex value: " + cellsColor.ColorIndex);

            // Sonucu görselleştirmek için çalışma kitabını kaydedin
            try
            {
                workbook.Save("ColorIndexDemo.xlsx");
                Console.WriteLine("Workbook saved as ColorIndexDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


