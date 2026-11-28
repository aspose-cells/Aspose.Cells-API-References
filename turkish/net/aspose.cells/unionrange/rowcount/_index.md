---
title: "UnionRange.RowCount"
second_title: "Aspose.Cells için .NET API Referansı"
description: "UnionRange özelliği. Aralıktaki satır sayısını alır"
type: docs
url: /tr/net/aspose.cells/unionrange/rowcount/
---
## UnionRange.RowCount property

Aralıktaki satır sayısını alır.

```csharp
public int RowCount { get; }
```

### Açıklamalar

Yalnızca bir aralık içerdiğinde etkili olur.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyRowCountDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına veri doldurun
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    worksheet.Cells[row, col].Value = $"Data {row},{col}";
                }
            }

            // A1'den E5'e bir birleşim aralığı oluşturun
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:E5");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A6:E10");
            UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

            // RowCount özelliğini göster
            Console.WriteLine("RowCount of union range: " + unionRange.RowCount);

            // Satırlar arasında yineleme yaparak kullanımı gösterin
            for (int i = 0; i < unionRange.RowCount; i++)
            {
                Aspose.Cells.Range currentRow = worksheet.Cells.CreateRange(
                    unionRange.FirstRow + i,
                    unionRange.FirstColumn,
                    1,
                    unionRange.ColumnCount);

                Console.WriteLine($"Row {i + 1} first cell value: " + currentRow[0, 0].Value);
            }

            // Farklı satır sayısına sahip yeni bir aralık oluşturun
            Aspose.Cells.Range newRange = worksheet.Cells.CreateRange("A1:E3");
            Console.WriteLine("RowCount of new range: " + newRange.RowCount);

            // Satır sayısına göre biçimlendirme uygulayın
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightYellow;
            style.Pattern = BackgroundType.Solid;

            for (int i = 0; i < unionRange.RowCount; i += 2)
            {
                Aspose.Cells.Range rowRange = worksheet.Cells.CreateRange(
                    unionRange.FirstRow + i,
                    unionRange.FirstColumn,
                    1,
                    unionRange.ColumnCount);
                rowRange.ApplyStyle(style, new StyleFlag { FontBold = true, CellShading = true });
            }

            // Çalışma kitabını kaydedin
            workbook.Save("UnionRangeRowCountDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


