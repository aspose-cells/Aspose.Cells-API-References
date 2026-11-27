---
title: "TxtSaveOptions.ExportArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtSaveOptions egenskap. Intervallet av celler som ska exporteras"
type: docs
url: /sv/net/aspose.cells/txtsaveoptions/exportarea/
---
## TxtSaveOptions.ExportArea property

Intervallet av celler som ska exporteras.

```csharp
public CellArea ExportArea { get; set; }
```

### Anmärkningar

Om det exporterade området har angetts, kommer [`TrimLeadingBlankRowAndColumn`](../trimleadingblankrowandcolumn/) inte att ha någon effekt.

### Exempel

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll celler med data
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(699.99);
            worksheet.Cells["A4"].PutValue("Tablet");
            worksheet.Cells["B4"].PutValue(399.99);

            // Konfigurera text sparalternativ med ExportArea
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Separator = '\t',
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 }
            };

            // Spara endast det angivna området (första 3 raderna, första 2 kolumnerna)
            workbook.Save("ExportedData.txt", saveOptions);

            Console.WriteLine("Data exported successfully with ExportArea restriction.");
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


