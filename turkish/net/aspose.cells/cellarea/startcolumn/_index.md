---
title: "CellArea.StartColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellArea alanı. Bu alanın başlangıç sütununu alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/cellarea/startcolumn/
---
## CellArea.StartColumn field

Bu alanın başlangıç sütununu alır veya ayarlar.

```csharp
public int StartColumn;
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaFieldStartColumnDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Bazı başlangıç verilerini ayarla
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue(10);
            cells["A3"].PutValue(20);

            // Bir CellArea oluştur ve StartColumn değerini ayarla
            CellArea area = new CellArea();
            area.StartRow = 1;
            area.EndRow = 3;
            area.StartColumn = 0; // Using StartColumn field
            area.EndColumn = 0;

            // Mevcut hücreleri aşağı kaydırarak yeni bir sütun ekle
            cells.InsertRange(area, ShiftType.Down);

            // Sonucu doğrula
            Console.WriteLine("A1 value: " + cells["A1"].StringValue); // Should be empty
            Console.WriteLine("A2 value: " + cells["A2"].StringValue); // Should be "Header"
            Console.WriteLine("A3 value: " + cells["A3"].IntValue); // Should be 10
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


