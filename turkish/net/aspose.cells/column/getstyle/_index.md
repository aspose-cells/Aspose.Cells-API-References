---
title: "Column.GetStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Column metodu. Bu sütunun stilini alır"
type: docs
url: /tr/net/aspose.cells/column/getstyle/
---
## Column.GetStyle method

Bu sütunun stilini alır.

```csharp
public Style GetStyle()
```

### Açıklamalar

Dönen stil nesnesini doğrudan değiştirmek bu sütun veya bu sütundaki hücreler için hiçbir etki oluşturmaz. Değişikliği bu sütuna uygulamak için [`ApplyStyle`](../applystyle/) veya [`SetStyle`](../setstyle/) metodunu çağırmanız gerekir. Sütunun stili, bu sütundaki hücreler tarafından (özel stil ayarları olmayan, örneğin stil açıkça ayarlanmamış mevcut hücreler veya henüz oluşturulmamış hücreler) devralınacak stildir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnMethodGetStyleDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Sütun 5 için stil ayarla
            Style columnStyle = cells.Columns[5].GetStyle();
            columnStyle.Font.Name = "Arial";
            columnStyle.Font.Size = 14;
            columnStyle.Font.IsBold = true;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { Font = true });

            // Satır 7 için stil ayarla
            Style rowStyle = cells.Rows[7].GetStyle();
            rowStyle.Font.Color = System.Drawing.Color.Red;
            rowStyle.Font.IsItalic = true;
            cells.Rows[7].ApplyStyle(rowStyle, new StyleFlag { Font = true });

            // Sütun stilini doğrula
            Style retrievedColumnStyle = cells.Columns[5].GetStyle();
            Console.WriteLine("Column 5 Style:");
            Console.WriteLine($"Font: {retrievedColumnStyle.Font.Name}, Size: {retrievedColumnStyle.Font.Size}, Bold: {retrievedColumnStyle.Font.IsBold}");

            // Satır stilini doğrula
            Style retrievedRowStyle = cells.Rows[7].GetStyle();
            Console.WriteLine("\nRow 7 Style:");
            Console.WriteLine($"Color: {retrievedRowStyle.Font.Color}, Italic: {retrievedRowStyle.Font.IsItalic}");

            // Çalışma kitabını kaydedin
            workbook.Save("ColumnMethodGetStyleDemo_output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


