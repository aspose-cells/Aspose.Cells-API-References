---
title: "WebExtensionTaskPane.IsLocked"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebExtensionTaskPane. تشير إلى ما إذا كانت لوحة المهام مقفلة على المستند في واجهة المستخدم ولا يمكن للمستخدم إغلاقها"
type: docs
url: /ar/net/aspose.cells.webextensions/webextensiontaskpane/islocked/
---
## WebExtensionTaskPane.IsLocked property

يشير إلى ما إذا كانت لوحة المهام مقفلة بالمستند في واجهة المستخدم ولا يمكن إغلاقها من قبل المستخدم.

```csharp
public bool IsLocked { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionTaskPanePropertyIsLockedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            try
            {
                // إنشاء لوحة مهام عبر مجموعة امتدادات الويب في دفتر العمل
                WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
                int paneIndex = taskPanes.Add();
                WebExtensionTaskPane taskPane = taskPanes[paneIndex];
                
                Console.WriteLine("Initial IsLocked value: " + taskPane.IsLocked);
                
                taskPane.IsLocked = true;
                Console.WriteLine("Updated IsLocked value: " + taskPane.IsLocked);

                workbook.Save("WebExtensionTaskPaneDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


