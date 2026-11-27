---
title: "WebExtensionTaskPane.Row"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebExtensionTaskPane-egenskap. Hämtar och anger index som räknar från utsidan till insidan av denna uppgiftspanel bland andra beständiga uppgiftspaneler som är dockade på samma standardplats."
type: docs
url: /sv/net/aspose.cells.webextensions/webextensiontaskpane/row/
---
## WebExtensionTaskPane.Row property

Hämtar och sätter indexet, räknat från utsidan till insidan, för detta taskpane bland andra beständiga taskpanes som är dockade på samma standardplats.

```csharp
public int Row { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionTaskPanePropertyRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett webbtillägg
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int webExtIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[webExtIndex];
            
            // Konfigurera egenskaper för webbtillägg
            webExt.Reference.Version = "1.0.0";
            webExt.Reference.StoreName = @"C:\Extensions\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            
            // Lägg till en uppgiftspanel
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];
            
            // Konfigurera uppgiftspanelens egenskaper
            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 300;
            
            // Demonstrera användning av Row-egenskapen
            taskPane.Row = 5; // Set row position
            
            // Spara arbetsboken
            workbook.Save("WebExtensionTaskPaneDemo.xlsx");
            
            Console.WriteLine("Workbook saved with web extension task pane (Row: " + taskPane.Row + ")");
        }
    }
}
```

### Se även

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


