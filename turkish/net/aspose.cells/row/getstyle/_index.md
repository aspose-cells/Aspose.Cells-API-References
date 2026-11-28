---
title: "Row.GetStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Row yöntemi. Bu satırın stilini alır"
type: docs
url: /tr/net/aspose.cells/row/getstyle/
---
## Row.GetStyle method

Bu satırın stilini alır.

```csharp
public Style GetStyle()
```

### Açıklamalar

İade edilen stil nesnesini doğrudan değiştirmek bu satır veya bu satırdaki hücreler üzerinde hiçbir etki yapmaz. Değişikliği bu satıra uygulamak için [`ApplyStyle`](../applystyle/) veya [`SetStyle`](../setstyle/) yöntemini çağırmanız gerekir. Satırın stili, bu satırdaki hücreler tarafından (özel stil ayarı olmayan hücreler, örneğin stil açıkça ayarlanmamış mevcut hücreler veya henüz oluşturulmamış hücreler) devralınacak stildir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Gösterim için stilleri ayarla
            Style rowStyle = workbook.CreateStyle();
            rowStyle.Pattern = BackgroundType.Solid;
            rowStyle.ForegroundColor = System.Drawing.Color.Blue;
            cells.Rows[8].ApplyStyle(rowStyle, new StyleFlag { All = true });

            Style columnStyle = workbook.CreateStyle();
            columnStyle.Pattern = BackgroundType.Solid;
            columnStyle.ForegroundColor = System.Drawing.Color.Red;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { All = true });

            // GetStyle kullanımını göster
            Style retrievedRowStyle = cells.Rows[8].GetStyle();
            Console.WriteLine("Row 8 Style - ForegroundColor: " + retrievedRowStyle.ForegroundColor);
            Console.WriteLine("Row 8 Style - Pattern: " + retrievedRowStyle.Pattern);

            Style retrievedColumnStyle = cells.Columns[5].GetStyle();
            Console.WriteLine("Column 5 Style - ForegroundColor: " + retrievedColumnStyle.ForegroundColor);
            Console.WriteLine("Column 5 Style - Pattern: " + retrievedColumnStyle.Pattern);
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


