---
title: "Cells.Columns"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Çalışma sayfasındaki bireysel sütunları temsil eden Column nesnelerinin koleksiyonunu alır"
type: docs
url: /tr/net/aspose.cells/cells/columns/
---
## Cells.Columns property

Çalışma sayfasındaki bireysel sütunları temsil eden [`Column`](../../column/) nesnelerinin koleksiyonunu alır.

```csharp
public ColumnCollection Columns { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyColumnsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Sütun 5 için stil ayarla
            Style columnStyle = workbook.CreateStyle();
            columnStyle.Font.Name = "Arial";
            columnStyle.Font.Size = 12;
            columnStyle.Font.IsBold = true;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { FontName = true, FontSize = true, FontBold = true });

            // Sütun 5 için genişlik ayarla
            cells.Columns[5].Width = 20;

            // Stili göstermek için sütun 5'te veri ayarla
            for (int row = 0; row < 10; row++)
            {
                cells[row, 5].PutValue($"Row {row + 1}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ColumnsPropertyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ColumnCollection](../../columncollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


