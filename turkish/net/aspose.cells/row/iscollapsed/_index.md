---
title: "Row.IsCollapsed"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Satır özelliği. Satırın daraltılmış olup olmadığını gösterir."
type: docs
url: /tr/net/aspose.cells/row/iscollapsed/
---
## Row.IsCollapsed property

Satırın katlanmış olup olmadığını gösterir.

```csharp
public bool IsCollapsed { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsCollapsedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir satır oluşturun ve stil verin
            Row row = worksheet.Cells.Rows[0];
            row.Height = 20;
            row.GroupLevel = 1;
            
            // IsCollapsed özelliğini gösterin
            row.IsCollapsed = true;
            Console.WriteLine("Row is collapsed: " + row.IsCollapsed);

            // Satırı genişletin
            row.IsCollapsed = false;
            Console.WriteLine("Row is collapsed: " + row.IsCollapsed);

            // Çalışma kitabını kaydedin
            workbook.Save("RowIsCollapsedDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


