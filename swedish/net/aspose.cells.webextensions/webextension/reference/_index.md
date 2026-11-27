---
title: "WebExtension.Reference"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebExtension egenskap. Hämtar den primära referensen till ett Office Addin"
type: docs
url: /sv/net/aspose.cells.webextensions/webextension/reference/
---
## WebExtension.Reference property

Hämta den primära referensen till ett Office-tillägg.

```csharp
public WebExtensionReference Reference { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionPropertyReferenceDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett webbtillägg
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int webExtIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[webExtIndex];
            
            // Ange referensegenskaper
            webExt.Reference.Version = "1.0.6.28";
            webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            
            // Lägg till tilläggsegenskaper
            webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");
            
            // Lägg till task pane
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int taskPaneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[taskPaneIndex];
            
            // Konfigurera task pane
            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 350;
            taskPane.Row = 7;
            
            // Spara arbetsboken
            workbook.Save("WebExtensionDemo.xlsx");
            
            Console.WriteLine("Web extension with reference properties created successfully.");
        }
    }
}
```

### Se även

* class [WebExtensionReference](../../webextensionreference/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


