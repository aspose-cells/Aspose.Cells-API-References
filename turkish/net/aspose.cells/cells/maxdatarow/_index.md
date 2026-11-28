---
title: "Cells.MaxDataRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Veri içeren hücrenin maksimum satır indeksi"
type: docs
url: /tr/net/aspose.cells/cells/maxdatarow/
---
## Cells.MaxDataRow property

Veri içeren hücrenin maksimum satır indeksi.

```csharp
public int MaxDataRow { get; }
```

### Açıklamalar

Veri içeren hücre yoksa -1 döndürür. Bu özellik hücreleri ve satırları dinamik olarak yinelemek ve kontrol etmek gerektiğinden zaman alıcı bir işlemdir ve bir döngüde doğrudan koşul olarak kullanmak gibi tekrarlı çağrılmamalıdır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxDataRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["A4"].PutValue("Item3");
            sheet.Cells["B4"].PutValue(30);

            // MaxDataRow kullanımını gösterin
            int maxRow = sheet.Cells.MaxDataRow;
            Console.WriteLine("Max data row: " + maxRow);

            // MaxDataRow kullanarak bir hücre alanı oluşturun
            int startRow = 0;
            int startColumn = 0;
            int endRow = sheet.Cells.MaxDataRow;
            int endColumn = sheet.Cells.MaxDataColumn;

            // Veri aralığına biçimlendirme uygula
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            
            // Stili aralığa uygulayın
            sheet.Cells.CreateRange(startRow, startColumn, endRow + 1, endColumn + 1).ApplyStyle(style, new StyleFlag { FontBold = true });

            // Çalışma kitabını kaydedin
            workbook.Save("MaxDataRowDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


