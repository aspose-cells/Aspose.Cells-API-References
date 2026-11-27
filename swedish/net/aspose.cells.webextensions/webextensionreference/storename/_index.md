---
title: "WebExtensionReference.StoreName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebExtensionReference-egenskap. Hämtar och anger instansen av marknadsplatsen där Office Addin lagras."
type: docs
url: /sv/net/aspose.cells.webextensions/webextensionreference/storename/
---
## WebExtensionReference.StoreName property

Hämtar och anger instansen av marknadsplatsen där Office-tillägget lagras. .

```csharp
public string StoreName { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionReferencePropertyStoreNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett webbtillägg
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int extensionIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[extensionIndex];
            
            // Ställ in web extension-referensegenskaper inklusive StoreName
            webExt.Reference.Version = "1.0.6.28";
            webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");

            // Lägg till en uppgiftspanel för web extension
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];

            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 350;

            // Spara arbetsboken
            workbook.Save("WebExtensionDemo.xlsx");
            
            Console.WriteLine("Workbook with web extension saved successfully.");
        }
    }
}
```

### Se även

* class [WebExtensionReference](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


