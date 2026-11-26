---
title: "PageSetup.CenterHorizontally"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Indica si la hoja se imprime centrada horizontalmente"
type: docs
url: /es/net/aspose.cells/pagesetup/centerhorizontally/
---
## PageSetup.CenterHorizontally property

Representa si la hoja se imprime centrada horizontalmente.

```csharp
public bool CenterHorizontally { get; set; }
```

### Ejemplos

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

            // Poblar algunos datos de muestra
            worksheet.Cells["A1"].PutValue("Sample Data");
            for (int i = 1; i <= 5; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Item " + i);
                worksheet.Cells["B" + (i + 1)].PutValue(i * 100);
            }

            PageSetup pageSetup = worksheet.PageSetup;
            
            // Demostrar la propiedad CenterHorizontally
            pageSetup.CenterHorizontally = true;
            pageSetup.PrintArea = "A1:B6";

            workbook.Save("CenterHorizontallyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


