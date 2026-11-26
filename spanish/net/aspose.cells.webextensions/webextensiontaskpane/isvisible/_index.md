---
title: "WebExtensionTaskPane.IsVisible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebExtensionTaskPane. Indica si el Task Pane se muestra visible por defecto cuando se abre el documento"
type: docs
url: /es/net/aspose.cells.webextensions/webextensiontaskpane/isvisible/
---
## WebExtensionTaskPane.IsVisible property

Indica si el Panel de tareas se muestra visible por defecto cuando se abre el documento.

```csharp
public bool IsVisible { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionTaskPanePropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una extensión web
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int extensionIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[extensionIndex];
            
            // Configurar propiedades de la extensión web
            webExt.Reference.Version = "1.0.0";
            webExt.Reference.StoreName = @"C:\\Extensions\\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            
            // Agregar un panel de tareas
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];
            
            // Configurar propiedades del panel de tareas
            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.Width = 300;
            
            // Demostrar la propiedad IsVisible
            Console.WriteLine("Initial IsVisible: " + taskPane.IsVisible);
            taskPane.IsVisible = true;
            Console.WriteLine("After setting to true: " + taskPane.IsVisible);
            
            // Guarda el libro de trabajo
            workbook.Save("WebExtensionTaskPaneDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


