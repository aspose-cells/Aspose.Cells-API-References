---
title: "WebExtensionTaskPane.IsLocked"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebExtensionTaskPane-egenskap. Anger om uppgiftspanelen är låst till dokumentet i UI och inte kan stängas av användaren"
type: docs
url: /sv/net/aspose.cells.webextensions/webextensiontaskpane/islocked/
---
## WebExtensionTaskPane.IsLocked property

Anger om taskpane är låst till dokumentet i UI och inte kan stängas av användaren.

```csharp
public bool IsLocked { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionTaskPanePropertyIsLockedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            try
            {
                // Skapa uppgiftspanel via arbetsbokens web extension-samling
                WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
                int paneIndex = taskPanes.Add();
                WebExtensionTaskPane taskPane = taskPanes[paneIndex];
                
                Console.WriteLine("Initial IsLocked value: " + taskPane.IsLocked);
                
                taskPane.IsLocked = true;
                Console.WriteLine("Updated IsLocked value: " + taskPane.IsLocked);

                workbook.Save("WebExtensionTaskPaneDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


