---
title: "Column.HasCustomStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Column özelliği. Bu sütunun, çalışma kitabından devralınan varsayılan stilden farklı özel stil ayarlarına sahip olup olmadığını gösterir."
type: docs
url: /tr/net/aspose.cells/column/hascustomstyle/
---
## Column.HasCustomStyle property

Bu sütunun, çalışma kitabından devralınan varsayılan ayardan farklı özel stil ayarlarına sahip olup olmadığını gösterir.

```csharp
public bool HasCustomStyle { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // İlk sütuna eriş
            Column column = worksheet.Cells.Columns[0];

            // İlk HasCustomState değerini göster
            Console.WriteLine("Initial HasCustomStyle: " + column.HasCustomStyle);

            // HasCustomStyle değişimini göstermek için sütun stilini değiştir
            Style columnStyle = column.GetStyle();
            columnStyle.BackgroundColor = Color.LightBlue;
            column.SetStyle(columnStyle);

            // Güncellenmiş HasCustomStyle değerini göster
            Console.WriteLine("After style modification - HasCustomStyle: " + column.HasCustomStyle);

            // Karşılaştırma için varsayılan stil ile başka bir sütun oluştur
            Column secondColumn = worksheet.Cells.Columns[1];
            Console.WriteLine("Second column HasCustomStyle: " + secondColumn.HasCustomStyle);

            // Çalışma kitabını kaydedin
            workbook.Save("ColumnHasCustomStyleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


