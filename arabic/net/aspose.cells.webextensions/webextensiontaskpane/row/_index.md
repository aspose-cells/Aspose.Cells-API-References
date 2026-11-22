---
title: "WebExtensionTaskPane.Row"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebExtensionTaskPane. تحصل وتضبط الفهرس الذي يعدد من الخارج إلى الداخل لهذه اللوحة بين لوحات المهام الأخرى المستمرة المثبتة في نفس الموقع الافتراضي"
type: docs
url: /ar/net/aspose.cells.webextensions/webextensiontaskpane/row/
---
## WebExtensionTaskPane.Row property

يحصل ويضبط الفهرس، مع العد من الخارج إلى الداخل، لهذه اللوحة الجانبية بين اللوحات الجانبية المستمرة الأخرى المثبتة في نفس الموقع الافتراضي.

```csharp
public int Row { get; set; }
```

### أمثلة

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
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة امتداد ويب
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int webExtIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[webExtIndex];
            
            // تكوين خصائص امتداد الويب
            webExt.Reference.Version = "1.0.0";
            webExt.Reference.StoreName = @"C:\Extensions\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            
            // إضافة لوحة مهام
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];
            
            // تكوين خصائص لوحة المهام
            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 300;
            
            // أظهر استخدام خاصية Row
            taskPane.Row = 5; // Set row position
            
            // احفظ المصنف
            workbook.Save("WebExtensionTaskPaneDemo.xlsx");
            
            Console.WriteLine("Workbook saved with web extension task pane (Row: " + taskPane.Row + ")");
        }
    }
}
```

### انظر أيضًا

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


