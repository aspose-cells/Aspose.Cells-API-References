---
title: "WebExtensionTaskPane.WebExtension"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebExtensionTaskPane. تحصل وتضبط جزء web extension المرتبط بمثيل taskpane"
type: docs
url: /ar/net/aspose.cells.webextensions/webextensiontaskpane/webextension/
---
## WebExtensionTaskPane.WebExtension property

يحصل ويضبط جزء الامتداد الويب المرتبط بمثيل اللوحة الجانبية

```csharp
public WebExtension WebExtension { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionTaskPanePropertyWebExtensionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int extensionIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[extensionIndex];
            
            webExt.Reference.Version = "1.0.0";
            webExt.Reference.StoreName = @"C:\Extensions\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");

            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];

            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 300;

            workbook.Save("WebExtensionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WebExtension](../../webextension/)
* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


