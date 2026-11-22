---
title: "WebExtensionReference.StoreName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebExtensionReference. تحصل وتضبط نسخة السوق حيث يتم تخزين إضافة Office."
type: docs
url: /ar/net/aspose.cells.webextensions/webextensionreference/storename/
---
## WebExtensionReference.StoreName property

يحصل ويضبط نسخة السوق التي تُخزن فيها إضافة Office.

```csharp
public string StoreName { get; set; }
```

### أمثلة

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
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة امتداد ويب
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int extensionIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[extensionIndex];
            
            // تعيين خصائص مرجع امتداد الويب بما في ذلك StoreName
            webExt.Reference.Version = "1.0.6.28";
            webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");

            // إضافة لوحة مهام لامتداد الويب
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];

            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 350;

            // احفظ المصنف
            workbook.Save("WebExtensionDemo.xlsx");
            
            Console.WriteLine("Workbook with web extension saved successfully.");
        }
    }
}
```

### انظر أيضًا

* class [WebExtensionReference](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


