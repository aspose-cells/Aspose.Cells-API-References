---
title: "WorksheetCollection.WebExtensionTaskPanes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorksheetCollection. تحصل على قائمة ألواح المهام"
type: docs
url: /ar/net/aspose.cells/worksheetcollection/webextensiontaskpanes/
---
## WorksheetCollection.WebExtensionTaskPanes property

يحصل على قائمة ألواح المهام.

```csharp
public WebExtensionTaskPaneCollection WebExtensionTaskPanes { get; }
```

### أمثلة

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
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة امتداد ويب
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int webExtIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[webExtIndex];
            
            // تكوين خصائص امتداد الويب
            webExt.Reference.Version = "1.0.6.28";
            webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");

            // إضافة وتكوين لوحة المهام
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int taskPaneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[taskPaneIndex];
            
            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 350;
            taskPane.Row = 7;

            // احفظ المصنف
            workbook.Save("WebExtensionTaskPaneDemo.xlsx");
            
            Console.WriteLine("Workbook with web extension task pane created successfully.");
        }
    }
}
```

### انظر أيضًا

* class [WebExtensionTaskPaneCollection](../../../aspose.cells.webextensions/webextensiontaskpanecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


