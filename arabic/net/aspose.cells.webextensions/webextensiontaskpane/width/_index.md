---
title: "WebExtensionTaskPane.Width"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebExtensionTaskPane. تحصل وتضبط قيمة العرض الافتراضية لهذه النسخة من لوحة المهام"
type: docs
url: /ar/net/aspose.cells.webextensions/webextensiontaskpane/width/
---
## WebExtensionTaskPane.Width property

يحصل ويضبط قيمة العرض الافتراضية لهذه اللوحة الجانبية.

```csharp
public double Width { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionTaskPanePropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            
            webExt.Reference.Version = "1.0.6.28";
            webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");

            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int taskPaneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[taskPaneIndex];

            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            
            // إظهار استخدام خاصية Width
            taskPane.Width = 350;
            
            workbook.Save("WebExtensionTaskPanePropertyWidthDemo.xlsx");
            
            Console.WriteLine("Workbook saved with task pane width set to: " + taskPane.Width);
        }
    }
}
```

### انظر أيضًا

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


