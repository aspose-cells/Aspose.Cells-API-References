---
title: "Cells.MaxDisplayRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Veri birleştirilmiş hücreleri ve şekilleri içeren en büyük aralığı alır"
type: docs
url: /tr/net/aspose.cells/cells/maxdisplayrange/
---
## Cells.MaxDisplayRange property

Veri, birleştirilmiş hücreler ve şekilleri içeren maksimum aralığı alır.

```csharp
public Range MaxDisplayRange { get; }
```

### Açıklamalar

Çalışma sayfası boş ise Aspose.Cells 21.5.2'den itibaren null döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxDisplayRangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere veri ekleyerek bir görüntüleme aralığı oluşturun
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(300);
            worksheet.Cells["B3"].PutValue(400);

            // En büyük görüntüleme aralığını alın
            Aspose.Cells.Range maxDisplayRange = worksheet.Cells.MaxDisplayRange;

            // Aralık bilgisini çıktı olarak verin
            Console.WriteLine("Max Display Range:");
            Console.WriteLine($"Start Row: {maxDisplayRange.FirstRow}");
            Console.WriteLine($"Start Column: {maxDisplayRange.FirstColumn}");
            Console.WriteLine($"Total Rows: {maxDisplayRange.RowCount}");
            Console.WriteLine($"Total Columns: {maxDisplayRange.ColumnCount}");

            // En büyük görüntüleme aralığının boyutlarına dayanarak yeni bir aralık oluşturun
            Aspose.Cells.Range customRange = worksheet.Cells.CreateRange(
                maxDisplayRange.FirstRow,
                maxDisplayRange.FirstColumn,
                maxDisplayRange.RowCount,
                maxDisplayRange.ColumnCount);

            // Aralığa biçimlendirme uygulayın
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightGray;
            style.Pattern = BackgroundType.Solid;
            customRange.ApplyStyle(style, new StyleFlag { FontBold = true, CellShading = true });

            // Çalışma kitabını kaydedin
            workbook.Save("MaxDisplayRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


