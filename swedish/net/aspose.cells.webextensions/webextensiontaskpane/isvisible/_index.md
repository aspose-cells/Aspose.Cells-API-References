---
title: "WebExtensionTaskPane.IsVisible"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebExtensionTaskPane-egenskap. Anger om Task Pane visas som synlig som standard när dokumentet öppnas"
type: docs
url: /sv/net/aspose.cells.webextensions/webextensiontaskpane/isvisible/
---
## WebExtensionTaskPane.IsVisible property

Anger om Task Pane visas som synlig som standard när dokumentet öppnas.

```csharp
public bool IsVisible { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionTaskPanePropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett webbtillägg
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int extensionIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[extensionIndex];
            
            // Konfigurera egenskaper för webbtillägg
            webExt.Reference.Version = "1.0.0";
            webExt.Reference.StoreName = @"C:\\Extensions\\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            
            // Lägg till en uppgiftspanel
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];
            
            // Konfigurera uppgiftspanelens egenskaper
            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.Width = 300;
            
            // Demonstrera IsVisible-egenskapen
            Console.WriteLine("Initial IsVisible: " + taskPane.IsVisible);
            taskPane.IsVisible = true;
            Console.WriteLine("After setting to true: " + taskPane.IsVisible);
            
            // Spara arbetsboken
            workbook.Save("WebExtensionTaskPaneDemo.xlsx");
        }
    }
}
```

### Se även

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


