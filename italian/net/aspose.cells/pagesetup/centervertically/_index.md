---
title: "PageSetup.CenterVertically"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Rappresenta se il foglio è stampato centrato verticalmente"
type: docs
url: /it/net/aspose.cells/pagesetup/centervertically/
---
## PageSetup.CenterVertically property

Rappresenta se il foglio viene stampato centrato verticalmente.

```csharp
public bool CenterVertically { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyCenterVerticallyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi a PageSetup e imposta CenterVertically
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.CenterVertically = true;
            
            // Aggiungi alcuni dati di esempio per visualizzare l'effetto
            worksheet.Cells["A1"].PutValue("This worksheet content will be centered vertically when printed");
            worksheet.Cells["A2"].PutValue("CenterVertically = true");
            
            // Salva la cartella di lavoro
            workbook.Save("PageSetup_CenterVertically.xlsx");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


