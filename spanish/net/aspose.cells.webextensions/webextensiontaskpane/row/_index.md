---
title: "WebExtensionTaskPane.Row"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebExtensionTaskPane. Obtiene y establece el índice que enumera de fuera hacia dentro este panel de tareas entre otros paneles de tareas persistentes acoplados en la misma ubicación predeterminada"
type: docs
url: /es/net/aspose.cells.webextensions/webextensiontaskpane/row/
---
## WebExtensionTaskPane.Row property

Obtiene y establece el índice, enumerando de fuera a dentro, de este panel de tareas entre otros paneles de tareas persistentes acoplados en la misma ubicación predeterminada.

```csharp
public int Row { get; set; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una extensión web
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int webExtIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[webExtIndex];
            
            // Configurar propiedades de la extensión web
            webExt.Reference.Version = "1.0.0";
            webExt.Reference.StoreName = @"C:\Extensions\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            
            // Agregar un panel de tareas
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];
            
            // Configurar propiedades del panel de tareas
            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 300;
            
            // Demostrar el uso de la propiedad Row
            taskPane.Row = 5; // Set row position
            
            // Guarda el libro de trabajo
            workbook.Save("WebExtensionTaskPaneDemo.xlsx");
            
            Console.WriteLine("Workbook saved with web extension task pane (Row: " + taskPane.Row + ")");
        }
    }
}
```

### Ver también

* class [WebExtensionTaskPane](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


