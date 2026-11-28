---
title: "Column.IsCollapsed"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Column özelliği. Sütunun daraltılmış olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/column/iscollapsed/
---
## Column.IsCollapsed property

sütunun daraltılıp daraltılmadığı

```csharp
public bool IsCollapsed { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ColumnPropertyIsCollapsedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sütuna basit bir stil oluşturun ve uygulayın
            Style style = workbook.CreateStyle();
            style.BackgroundColor = Color.LightGray;
            
            Column column = worksheet.Cells.Columns[0];
            column.ApplyStyle(style, new StyleFlag { All = true });

            // IsCollapsed dahil olmak üzere sütun özelliklerini ayarlayın
            column.Width = 15;
            column.IsCollapsed = true; // Demonstrating IsCollapsed property
            column.IsHidden = false;

            // Katlanmış sütunu görselleştirmek için bazı veriler ekleyin
            worksheet.Cells["A1"].PutValue("Collapsed Column");
            worksheet.Cells["B1"].PutValue("Visible Column");

            workbook.Save("ColumnIsCollapsedDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


