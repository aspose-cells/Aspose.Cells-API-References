---
title: "Cell.Column"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Hücrenin sıfır tabanlı sütun numarasını alır"
type: docs
url: /tr/net/aspose.cells/cell/column/
---
## Cell.Column property

Hücrenin sütun numarasını (sıfır tabanlı) alır.

```csharp
public int Column { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyColumnDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere erişin ve Column özelliğini gösterin
            Cell cell1 = worksheet.Cells["A1"];
            Cell cell2 = worksheet.Cells["B2"];
            Cell cell3 = worksheet.Cells["C3"];

            // Değerleri ve stilleri ayarlayın
            cell1.PutValue("Cell A1");
            cell2.PutValue("Cell B2");
            cell3.PutValue("Cell C3");

            // Column özelliğinin kullanımını gösterin
            Console.WriteLine("Cell A1 is in column: " + cell1.Column);
            Console.WriteLine("Cell B2 is in column: " + cell2.Column);
            Console.WriteLine("Cell C3 is in column: " + cell3.Column);

            // Column özelliğini kullanarak sütun genişliğini değiştirin
            worksheet.Cells.Columns[cell1.Column].Width = 20;
            worksheet.Cells.Columns[cell2.Column].Width = 25;
            worksheet.Cells.Columns[cell3.Column].Width = 30;

            // Çalışma kitabını kaydedin
            workbook.Save("ColumnPropertyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


