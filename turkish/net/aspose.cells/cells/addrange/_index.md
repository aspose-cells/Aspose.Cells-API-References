---
title: "Cells.AddRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Bir range nesnesi referansını hücrelere ekler."
type: docs
url: /tr/net/aspose.cells/cells/addrange/
---
## Cells.AddRange method

Hücrelere bir aralık nesnesi referansı ekler.

```csharp
public void AddRange(Range rangeObject)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rangeObject | Aralık | Range nesnesi hücrelerde bulunacak. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodAddRangeWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Aralık içinde bazı örnek veriler ayarlayın.
            cells["A1"].PutValue("A1");
            cells["A2"].PutValue("A2");
            cells["B1"].PutValue("B1");
            cells["B2"].PutValue("B2");

            // AddRange kullanarak bir aralık oluşturun ve ekleyin.
            Aspose.Cells.Range range = cells.CreateRange("A1", "B2");
            cells.AddRange(range);

            // Aralık genişlemesini göstermek için çalışma sayfasını değiştirin.
            cells.InsertRow(1);
            cells.InsertColumn(1);

            Console.WriteLine($"Range now has {range.RowCount} rows and {range.ColumnCount} columns");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


