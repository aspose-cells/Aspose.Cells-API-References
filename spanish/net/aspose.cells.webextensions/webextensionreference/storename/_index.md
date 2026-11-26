---
title: "WebExtensionReference.StoreName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebExtensionReference. Obtiene y establece la instancia del marketplace donde se almacena el complemento de Office."
type: docs
url: /es/net/aspose.cells.webextensions/webextensionreference/storename/
---
## WebExtensionReference.StoreName property

Obtiene y establece la instancia del marketplace donde se almacena el complemento de Office.

```csharp
public string StoreName { get; set; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una extensión web
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int extensionIndex = webExtensions.Add();
            WebExtension webExt = webExtensions[extensionIndex];
            
            // Establecer propiedades de referencia de la extensión web, incluido StoreName
            webExt.Reference.Version = "1.0.6.28";
            webExt.Reference.StoreName = @"\\wanlink.us\DFSRoot\APPS\meZocliq\UAT\Excel_Addin\";
            webExt.Reference.StoreType = WebExtensionStoreType.FileSystem;
            webExt.Properties.Add("Office.AutoShowTaskpaneWithDocument", "true");

            // Agregar un panel de tareas para la extensión web
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            int paneIndex = taskPanes.Add();
            WebExtensionTaskPane taskPane = taskPanes[paneIndex];

            taskPane.WebExtension = webExt;
            taskPane.DockState = "right";
            taskPane.IsVisible = true;
            taskPane.Width = 350;

            // Guarda el libro de trabajo
            workbook.Save("WebExtensionDemo.xlsx");
            
            Console.WriteLine("Workbook with web extension saved successfully.");
        }
    }
}
```

### Ver también

* class [WebExtensionReference](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


