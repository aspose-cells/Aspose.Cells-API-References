---
title: "WebExtensionTaskPane.WebExtension"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebExtensionTaskPane. Obtiene y establece la parte de la extensión web asociada a la instancia del taskpane"
type: docs
url: /es/net/aspose.cells.webextensions/webextensiontaskpane/webextension/
---
## WebExtensionTaskPane.WebExtension property

Obtiene y establece la parte de extensión web asociada con la instancia del panel de tareas.

```csharp
public WebExtension WebExtension { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionTaskPanePropertyWebExtensionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int extensionIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[extensionIndex];
            
            webExt.Reference.Version = "1.0.0";
            webExt.Reference.StoreName = @"C:\Extensions\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");

            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];

            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 300;

            workbook.Save("WebExtensionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WebExtension](../../webextension/)
* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


