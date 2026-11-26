---
title: "WebExtensionTaskPane.DockState"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebExtensionTaskPane. Получает и задает последнее закрепленное расположение этого объекта панели задач"
type: docs
url: /ru/net/aspose.cells.webextensions/webextensiontaskpane/dockstate/
---
## WebExtensionTaskPane.DockState property

Получает и задает последнее закреплённое расположение этого объекта панели задач.

```csharp
public string DockState { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionTaskPanePropertyDockStateDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int extensionIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[extensionIndex];
            
            webExt.Reference.Version = "1.0.0";
            webExt.Reference.StoreName = @"C:\\Temp\\Addins\\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;

            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];

            taskPane.WebExtension = webExt;
            taskPane.DockState = "right"; // Demonstrating DockState property
            taskPane.IsVisible = true;
            taskPane.Width = 300;

            workbook.Save("WebExtensionTaskPaneDockStateDemo.xlsx");
        }
    }
}
```

### См. также

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


