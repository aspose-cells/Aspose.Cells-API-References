---
title: "WebExtensionTaskPaneCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebExtensionTaskPaneCollection. تحصل على لوحة المهام حسب الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells.webextensions/webextensiontaskpanecollection/item/
---
## WebExtensionTaskPaneCollection indexer

يحصل على لوحة المهام حسب الفهرس المحدد.

```csharp
public WebExtensionTaskPane this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس. |

### قيمة الإرجاع

لوحة المهام.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionTaskPaneCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int extensionIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[extensionIndex];
            
            webExt.Reference.Version = "1.0.0";
            webExt.Reference.StoreName = @"C:\\Extensions\\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            webExt.Properties.Add("Office.AutoShowTaskpane", "true");

            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];

            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 300;

            // عرض استخدام خاصية Item
            WebExtensionTaskPane retrievedPane = taskPanes[paneIndex];
            Console.WriteLine($"Retrieved task pane width: {retrievedPane.Width}");

            workbook.Save("WebExtensionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WebExtensionTaskPane](../../webextensiontaskpane/)
* class [WebExtensionTaskPaneCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


