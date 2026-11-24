---
title: "Enum ViewType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ViewType-Enum. Stellt den Ansichtstyp des Arbeitsblatts dar"
type: docs
url: /de/net/aspose.cells/viewtype/
---
## ViewType enumeration

Stellt den Ansichtstyp des Arbeitsblatts dar.

```csharp
public enum ViewType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| NormalView | `0` |  |
| PageBreakPreview | `1` |  |
| PageLayoutView | `2` |  |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ViewTypeDemo
    {
        public static void ViewTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setze den Ansichtstyp des Arbeitsblatts auf PageBreakPreview
            worksheet.ViewType = ViewType.PageBreakPreview;
            
            // Speichere die Arbeitsmappe
            workbook.Save("ViewTypeExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


