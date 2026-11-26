---
title: "WebExtensionTaskPane.Width"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebExtensionTaskPane. Получает и задает значение ширины по умолчанию для этого экземпляра панели задач"
type: docs
url: /ru/net/aspose.cells.webextensions/webextensiontaskpane/width/
---
## WebExtensionTaskPane.Width property

Получает и задает значение ширины по умолчанию для этого экземпляра панели задач.

```csharp
public double Width { get; set; }
```

### Примеры

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
            
            // Продемонстрировать использование свойства Width
            taskPane.Width = 350;
            
            workbook.Save("WebExtensionTaskPanePropertyWidthDemo.xlsx");
            
            Console.WriteLine("Workbook saved with task pane width set to: " + taskPane.Width);
        }
    }
}
```

### См. также

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


