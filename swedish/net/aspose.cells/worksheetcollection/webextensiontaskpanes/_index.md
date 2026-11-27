---
title: "WorksheetCollection.WebExtensionTaskPanes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-egenskap. Hämtar listan över uppgiftspaneler"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/webextensiontaskpanes/
---
## WorksheetCollection.WebExtensionTaskPanes property

Hämtar listan över uppgiftspaneler.

```csharp
public WebExtensionTaskPaneCollection WebExtensionTaskPanes { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyWebExtensionTaskPanesDemo
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
            webExt.Reference.Version = "1.0.6.28";
            webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");

            // Lägg till och konfigurera uppgiftspanelen
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int taskPaneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[taskPaneIndex];
            
            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 350;
            taskPane.Row = 7;

            // Spara arbetsboken
            workbook.Save("WebExtensionTaskPaneDemo.xlsx");
            
            Console.WriteLine("Workbook with web extension task pane created successfully.");
        }
    }
}
```

### Se även

* class [WebExtensionTaskPaneCollection](../../../aspose.cells.webextensions/webextensiontaskpanecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


