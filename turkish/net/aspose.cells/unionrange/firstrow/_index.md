---
title: "UnionRange.FirstRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "UnionRange özelliği. Aralığın ilk satırının indeksini alır"
type: docs
url: /tr/net/aspose.cells/unionrange/firstrow/
---
## UnionRange.FirstRow property

Aralığın ilk satırının indeksini alır.

```csharp
public int FirstRow { get; }
```

### Açıklamalar

Yalnızca bir aralık içerdiğinde etkili olur.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyFirstRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek verileri doldur
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    worksheet.Cells[row, col].Value = $"Row {row}, Col {col}";
                }
            }

            // A2:C5 ve A7:C9 aralıklarından bir birleşim aralığı oluşturun
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A2:C5");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A7:C9");
            UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

            // FirstRow özelliğini göster
            Console.WriteLine("FirstRow of union range: " + unionRange.FirstRow);

            // İlk satırı vurgulayarak kullanımını gösterin
            Style highlightStyle = workbook.CreateStyle();
            highlightStyle.Font.IsBold = true;
            highlightStyle.ForegroundColor = System.Drawing.Color.LightGreen;
            highlightStyle.Pattern = BackgroundType.Solid;

            Aspose.Cells.Range firstRowRange = worksheet.Cells.CreateRange(
                unionRange.FirstRow,
                unionRange.FirstColumn,
                1,
                unionRange.ColumnCount);
            firstRowRange.ApplyStyle(highlightStyle, new StyleFlag { FontBold = true, CellShading = true });

            // Başka bir aralık oluşturun ve FirstRow değerlerini karşılaştırın
            Aspose.Cells.Range singleRange = worksheet.Cells.CreateRange("D1:F5");
            Console.WriteLine("FirstRow of single range: " + singleRange.FirstRow);
            Console.WriteLine("Is union range starting after single range? " + 
                (unionRange.FirstRow > singleRange.FirstRow));

            // Çalışma kitabını kaydedin
            workbook.Save("UnionRangeFirstRowDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


