---
title: "Yapı CellArea"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.CellArea yapısı. Hücrelerin bir alanını temsil eder"
type: docs
url: /tr/net/aspose.cells/cellarea/
---
## CellArea structure

Hücrelerin bir alanını temsil eder.

```csharp
public struct CellArea : IComparable
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [CreateCellArea](../../aspose.cells/cellarea/createcellarea/#createcellarea_1)(string, string) | Bir hücre alanı oluşturur. |
| static [CreateCellArea](../../aspose.cells/cellarea/createcellarea/#createcellarea)(int, int, int, int) | Bir hücre alanı oluşturur. |
| [CompareTo](../../aspose.cells/cellarea/compareto/)(object) | İki CellArea nesnesini sol üst köşelerine göre karşılaştırın. |
| override [ToString](../../aspose.cells/cellarea/tostring/)() | Geçerli hücre alanı nesnesini temsil eden bir dize döndürür. |

## Alanlar

| Ad | Açıklama |
| --- | --- |
| [EndColumn](../../aspose.cells/cellarea/endcolumn/) | Bu alanın son sütununu alır veya ayarlar. |
| [EndRow](../../aspose.cells/cellarea/endrow/) | Bu alanın son satırını alır veya ayarlar. |
| [StartColumn](../../aspose.cells/cellarea/startcolumn/) | Bu alanın başlangıç sütununu alır veya ayarlar. |
| [StartRow](../../aspose.cells/cellarea/startrow/) | Bu alanın başlangıç satırını alır veya ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellAreaDemo
    {
        public static void CellAreaExample()
        {
            // Yeni bir Workbook oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B5"].PutValue(20);
            worksheet.Cells["B8"].PutValue(50);
            worksheet.Cells["C2"].PutValue(8);
            worksheet.Cells["C7"].PutValue(15);
            worksheet.Cells["C9"].PutValue(30);

            // Hücre Alanı Oluştur
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 10;
            ca.StartColumn = 0;
            ca.EndColumn = 10;

            // Çalışma sayfasına koşullu biçimlendirme kuralı ekle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "30");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Çalışma kitabını kaydedin
            workbook.Save("CellAreaExample.xlsx");
            workbook.Save("CellAreaExample.pdf");

            // ToString yöntemini göster
            Console.WriteLine(ca.ToString());

            // CompareTo yöntemini göster
            CellArea ca2 = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };
            int comparisonResult = ca.CompareTo(ca2);
            Console.WriteLine($"Comparison result: {comparisonResult}");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


