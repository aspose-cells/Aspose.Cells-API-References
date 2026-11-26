---
title: "WebExtensionTaskPane.DockState"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebExtensionTaskPane. Obtiene y establece la ubicación lastdocked de este objeto taskpane"
type: docs
url: /es/net/aspose.cells.webextensions/webextensiontaskpane/dockstate/
---
## WebExtensionTaskPane.DockState property

Obtiene y establece la última ubicación acoplada de este objeto de panel de tareas.

```csharp
public string DockState { get; set; }
```

### Ejemplos

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

### Ver también

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


