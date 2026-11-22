---
title: "WorksheetCollection.WebExtensions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorksheetCollection. تحصل على قائمة ألواح المهام"
type: docs
url: /ar/net/aspose.cells/worksheetcollection/webextensions/
---
## WorksheetCollection.WebExtensions property

يحصل على قائمة ألواح المهام.

```csharp
public WebExtensionCollection WebExtensions { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyWebExtensionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int extensionIndex = webExtensions.Add();
            
            WebExtension webExt = webExtensions[extensionIndex];
            webExt.Reference.Version = "1.0.6.28";
            webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");

            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];

            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 350;
            taskPane.Row = 7;

            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WebExtensionCollection](../../../aspose.cells.webextensions/webextensioncollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


