---
title: "PageSetup.CenterHorizontally"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Indica se il foglio è stampato centrato orizzontalmente"
type: docs
url: /it/net/aspose.cells/pagesetup/centerhorizontally/
---
## PageSetup.CenterHorizontally property

Rappresenta se il foglio viene stampato centrato orizzontalmente.

```csharp
public bool CenterHorizontally { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyCenterHorizontallyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola alcuni dati di esempio
            worksheet.Cells["A1"].PutValue("Sample Data");
            for (int i = 1; i <= 5; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Item " + i);
                worksheet.Cells["B" + (i + 1)].PutValue(i * 100);
            }

            PageSetup pageSetup = worksheet.PageSetup;
            
            // Dimostra la proprietà CenterHorizontally
            pageSetup.CenterHorizontally = true;
            pageSetup.PrintArea = "A1:B6";

            workbook.Save("CenterHorizontallyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


