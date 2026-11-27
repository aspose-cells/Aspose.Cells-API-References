---
title: "Workbook.Theme"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-egenskap. Hämtar temats namn"
type: docs
url: /sv/net/aspose.cells/workbook/theme/
---
## Workbook.Theme property

Hämtar temats namn.

```csharp
public string Theme { get; }
```

### Exempel

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
            
            // Visa hur man hämtar standardtemat
            Console.WriteLine("Default theme: " + workbook.Theme);
            
            // Ändra temafärg och verifiera
            workbook.SetThemeColor(ThemeColorType.Accent1, Color.Blue);
            Color accent1 = workbook.GetThemeColor(ThemeColorType.Accent1);
            Console.WriteLine("Modified Accent1 color: " + accent1);
            
            // Spara workbook för att demonstrera temapersistens
            workbook.Save("ThemeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


