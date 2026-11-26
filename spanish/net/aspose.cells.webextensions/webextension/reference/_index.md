---
title: "WebExtension.Reference"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebExtension. Obtenga la referencia principal a un complemento de Office"
type: docs
url: /es/net/aspose.cells.webextensions/webextension/reference/
---
## WebExtension.Reference property

Obtiene la referencia principal a un Office Add-in.

```csharp
public WebExtensionReference Reference { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionPropertyReferenceDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una extensión web
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int webExtIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[webExtIndex];
            
            // Establezca propiedades de referencia
            webExt.Reference.Version = "1.0.6.28";
            webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            
            // Agregue propiedades de extensión
            webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");
            
            // Agregue panel de tareas
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int taskPaneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[taskPaneIndex];
            
            // Configure el panel de tareas
            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 350;
            taskPane.Row = 7;
            
            // Guarda el libro de trabajo
            workbook.Save("WebExtensionDemo.xlsx");
            
            Console.WriteLine("Web extension with reference properties created successfully.");
        }
    }
}
```

### Ver también

* class [WebExtensionReference](../../webextensionreference/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


