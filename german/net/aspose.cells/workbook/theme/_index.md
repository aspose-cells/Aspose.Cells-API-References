---
title: "Workbook.Theme"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Eigenschaft. Gibt den Namen des Themas zurück"
type: docs
url: /de/net/aspose.cells/workbook/theme/
---
## Workbook.Theme property

Liest den Namen des Themas.

```csharp
public string Theme { get; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyThemeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Demonstration des Abrufs des Standardthemas
            Console.WriteLine("Default theme: " + workbook.Theme);
            
            // Themenfarbe ändern und überprüfen
            workbook.SetThemeColor(ThemeColorType.Accent1, Color.Blue);
            Color accent1 = workbook.GetThemeColor(ThemeColorType.Accent1);
            Console.WriteLine("Modified Accent1 color: " + accent1);
            
            // Speichere das Workbook, um die Themenpersistenz zu demonstrieren
            workbook.Save("ThemeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


