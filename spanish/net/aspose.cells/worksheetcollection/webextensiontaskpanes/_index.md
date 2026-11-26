---
title: "WorksheetCollection.WebExtensionTaskPanes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorksheetCollection. Obtiene la lista de paneles de tareas"
type: docs
url: /es/net/aspose.cells/worksheetcollection/webextensiontaskpanes/
---
## WorksheetCollection.WebExtensionTaskPanes property

Obtiene la lista de paneles de tareas.

```csharp
public WebExtensionTaskPaneCollection WebExtensionTaskPanes { get; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una extensión web
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int webExtIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[webExtIndex];
            
            // Configurar propiedades de la extensión web
            webExt.Reference.Version = "1.0.6.28";
            webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");

            // Agregar y configurar el panel de tareas
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int taskPaneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[taskPaneIndex];
            
            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 350;
            taskPane.Row = 7;

            // Guarda el libro de trabajo
            workbook.Save("WebExtensionTaskPaneDemo.xlsx");
            
            Console.WriteLine("Workbook with web extension task pane created successfully.");
        }
    }
}
```

### Ver también

* class [WebExtensionTaskPaneCollection](../../../aspose.cells.webextensions/webextensiontaskpanecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


