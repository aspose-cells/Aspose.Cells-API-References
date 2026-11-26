---
title: "WebExtensionTaskPane.Width"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebExtensionTaskPane. Obtiene y establece el valor de ancho predeterminado para esta instancia de panel de tareas"
type: docs
url: /es/net/aspose.cells.webextensions/webextensiontaskpane/width/
---
## WebExtensionTaskPane.Width property

Obtiene y establece el valor de ancho predeterminado para esta instancia del panel de tareas.

```csharp
public double Width { get; set; }
```

### Ejemplos

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
            
            // Demostrar el uso de la propiedad Width
            taskPane.Width = 350;
            
            workbook.Save("WebExtensionTaskPanePropertyWidthDemo.xlsx");
            
            Console.WriteLine("Workbook saved with task pane width set to: " + taskPane.Width);
        }
    }
}
```

### Ver también

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


