---
title: "FindOptions.SetRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FindOptions yöntemi. Aranan aralığı ayarlar"
type: docs
url: /tr/net/aspose.cells/findoptions/setrange/
---
## FindOptions.SetRange method

Aranan aralığı ayarlar.

```csharp
public void SetRange(CellArea ca)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ca | CellArea | aranan aralık. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsMethodSetRangeWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bazı verileri doldurun
            worksheet.Cells["A1"].PutValue("abc");
            worksheet.Cells["B2"].PutValue("def");
            worksheet.Cells["C3"].PutValue("abc");
            
            // FindOptions oluşturun ve arama aralığını ayarlayın
            FindOptions rangeOptions = new FindOptions();
            CellArea cellarea = new CellArea();
            cellarea.StartRow = 1;
            cellarea.StartColumn = 1;
            cellarea.EndRow = 3;
            cellarea.EndColumn = 3;
            rangeOptions.SetRange(cellarea);
            
            // Belirtilen aralık içinde arama yapın
            rangeOptions.SearchBackward = false;
            Cell foundCell = worksheet.Cells.Find("abc", null, rangeOptions);
            
            Console.WriteLine("Found 'abc' at row: " + foundCell.Row + ", column: " + foundCell.Column);
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


