---
title: "PageSetup.CenterVertically"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt an, ob das Blatt vertikal zentriert gedruckt wird."
type: docs
url: /de/net/aspose.cells/pagesetup/centervertically/
---
## PageSetup.CenterVertically property

Gibt an, ob das Blatt vertikal zentriert gedruckt wird.

```csharp
public bool CenterVertically { get; set; }
```

### Beispiele

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
            
            // Greife auf PageSetup zu und setze CenterVertically
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.CenterVertically = true;
            
            // Fügen Sie einige Beispieldaten hinzu, um die Wirkung zu visualisieren.
            worksheet.Cells["A1"].PutValue("This worksheet content will be centered vertically when printed");
            worksheet.Cells["A2"].PutValue("CenterVertically = true");
            
            // Speichere die Arbeitsmappe
            workbook.Save("PageSetup_CenterVertically.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


