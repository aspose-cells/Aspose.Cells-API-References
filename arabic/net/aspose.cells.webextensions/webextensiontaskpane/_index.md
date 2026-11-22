---
title: "الفئة WebExtensionTaskPane"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.WebExtensions.WebExtensionTaskPane. تمثل كائن لوحة مهام محفوظ"
type: docs
url: /ar/net/aspose.cells.webextensions/webextensiontaskpane/
---
## WebExtensionTaskPane class

يمثل كائن taskpane محفوظ.

```csharp
public class WebExtensionTaskPane
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [DockState](../../aspose.cells.webextensions/webextensiontaskpane/dockstate/) { get; set; } | يحصل ويضبط الموقع الأخير المثبت لهذا الكائن من لوحة المهام. |
| [IsLocked](../../aspose.cells.webextensions/webextensiontaskpane/islocked/) { get; set; } | يشير إلى ما إذا كانت لوحة المهام مقفلة بالمستند في واجهة المستخدم ولا يمكن إغلاقها من قبل المستخدم. |
| [IsVisible](../../aspose.cells.webextensions/webextensiontaskpane/isvisible/) { get; set; } | يشير إلى ما إذا كانت لوحة المهام تُظهر كمرئية افتراضيًا عند فتح المستند. |
| [Row](../../aspose.cells.webextensions/webextensiontaskpane/row/) { get; set; } | يحصل ويضبط الفهرس، مع العد من الخارج إلى الداخل، لهذه اللوحة الجانبية بين اللوحات الجانبية المستمرة الأخرى المثبتة في نفس الموقع الافتراضي. |
| [WebExtension](../../aspose.cells.webextensions/webextensiontaskpane/webextension/) { get; set; } | يحصل ويضبط جزء الامتداد الويب المرتبط بمثيل اللوحة الجانبية |
| [Width](../../aspose.cells.webextensions/webextensiontaskpane/width/) { get; set; } | يحصل ويضبط قيمة العرض الافتراضية لهذه اللوحة الجانبية. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionsClassWebExtensionTaskPaneDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int webExtIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[webExtIndex];
            
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
            taskPane.Width = 350;
            taskPane.Row = 7;

            workbook.Save("WebExtensionTaskPaneDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


